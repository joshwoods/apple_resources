

- ScreenCaptureKit
- SCStreamConfiguration
-  colorMatrix 

Instance Property

# colorMatrix

A color matrix to apply to the output surface.

Mac Catalyst 18.2+macOS 12.3+

``` source
unowned(unsafe) var colorMatrix: CFString { get set }
```

## Discussion

You can specify a value for this property if your pixel format is `420v` or `420f`. The value must be one of the strings specified in Display Stream YCbCr to RGB conversion Matrix Options.

## See Also

### Configuring colors

var pixelFormat: OSType

A pixel format for sample buffers that a stream outputs.

var colorSpaceName: CFString

A color space to use for the output buffer.

var backgroundColor: CGColor

A background color for the output.

