# 场景
通常我们会把一些不经常变化，但有经常使用的业务数据放到缓存中去，以提高性能。目前业界使用较多的是缓存中间件是memcache和redis，通常我们会在具体业务逻辑代码中使用他们提供的api进行缓存的操作，比如将数据放入缓存中，或从缓存中获取数据。

# 问题
上面的场景中业务逻辑和缓存逻辑是混在一起，假如未来有更好的缓存中间件可以使用，那么我们需要在所有之前使用过缓存的地方都进行修改。
