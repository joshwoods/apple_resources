

- AGL
-  AGL_CLEAR_FORMAT_CACHE 

Global Variable

# AGL_CLEAR_FORMAT_CACHE

macOS 10.0+

``` source
var AGL_CLEAR_FORMAT_CACHE: Int32 { get }
```

## Discussion

When the associated value is nonzero, specifies to reset the pixel format cache. Clearing the cache does not affect the size of the cache for future storage of pixel formats. To minimize the memory consumed by the cache, your application should also set the cache size to `1`.

## See Also

### Constants

var AGL_FORMAT_CACHE_SIZE: Int32

var AGL_RETAIN_RENDERERS: Int32

var AGL_FORMAT_CACHE_SIZE: Int32

var AGL_RETAIN_RENDERERS: Int32

