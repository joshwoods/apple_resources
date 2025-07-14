

- ScreenCaptureKit
- SCStreamConfiguration
-  pixelFormat 

Instance Property

# pixelFormat

A pixel format for sample buffers that a stream outputs.

Mac Catalyst 18.2+macOS 12.3+

``` source
var pixelFormat: OSType { get set }
```

## Discussion

A stream supports the following pixel formats:

`BGRA`  
Packed little endian ARGB8888.

`l10r`  
Packed little endian ARGB2101010.

`420v`  
Two-plane “video” range YCbCr 4:2:0.

`420f`  
Two-plane “full” range YCbCr 4:2:0.

## See Also

### Configuring colors

var colorMatrix: CFString

A color matrix to apply to the output surface.

var colorSpaceName: CFString

A color space to use for the output buffer.

var backgroundColor: CGColor

A background color for the output.

