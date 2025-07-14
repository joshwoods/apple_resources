

- AGL
-  AGL_RETAIN_RENDERERS 

Global Variable

# AGL_RETAIN_RENDERERS

macOS 10.0+

``` source
var AGL_RETAIN_RENDERERS: Int32 { get }
```

## Discussion

Specifies whether or not to retain loaded plug-in renderers in memory. When the associated value is nonzero, the AGL library will not unload any plug-in renderers even if they are no longer in use. This option is useful to improve the performance of applications that repeatedly destroy and recreate their only (or last) rendering context. Normally, when the last rendering context created by a particular plug-in renderer is destroyed, that renderer is unloaded from memory. When the associated value is zero, AGL returns to its normal mode of operation and all renderers that are not in use are unloaded.

## See Also

### Constants

var AGL_FORMAT_CACHE_SIZE: Int32

var AGL_CLEAR_FORMAT_CACHE: Int32

var AGL_FORMAT_CACHE_SIZE: Int32

var AGL_CLEAR_FORMAT_CACHE: Int32

