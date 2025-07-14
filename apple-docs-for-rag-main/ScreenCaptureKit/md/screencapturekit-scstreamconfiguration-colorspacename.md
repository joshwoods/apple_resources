

- ScreenCaptureKit
- SCStreamConfiguration
-  colorSpaceName 

Instance Property

# colorSpaceName

A color space to use for the output buffer.

Mac Catalyst 18.2+macOS 12.3+

``` source
unowned(unsafe) var colorSpaceName: CFString { get set }
```

## Discussion

If you don’t specify a value, the output buffer uses the same color space as the display. If you specify a value, if must be one of the strings specified in CGColorSpace.

## See Also

### Configuring colors

var pixelFormat: OSType

A pixel format for sample buffers that a stream outputs.

var colorMatrix: CFString

A color matrix to apply to the output surface.

var backgroundColor: CGColor

A background color for the output.

