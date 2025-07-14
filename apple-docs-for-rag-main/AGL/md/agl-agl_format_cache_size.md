

- AGL
-  AGL_FORMAT_CACHE_SIZE 

Global Variable

# AGL_FORMAT_CACHE_SIZE

macOS 10.0+

``` source
var AGL_FORMAT_CACHE_SIZE: Int32 { get }
```

## Discussion

The associated value is the size of the positive pixel format cache and is initially set to `5`. If your application needs to use `n` different attribute lists to choose `n` different pixel formats repeatedly, then the application should set the cache size to `n` to maximize performance. After your application calls the aglChoosePixelFormat function for the last time, you might want to set the cache size to `1` to minimize the memory used by the AGL library.

## See Also

### Constants

var AGL_CLEAR_FORMAT_CACHE: Int32

var AGL_RETAIN_RENDERERS: Int32

var AGL_CLEAR_FORMAT_CACHE: Int32

var AGL_RETAIN_RENDERERS: Int32

