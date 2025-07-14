

- Core Graphics
- CGContext
-  setStrokeColor(cyan:magenta:yellow:black:alpha:) 

Instance Method

# setStrokeColor(cyan:magenta:yellow:black:alpha:)

Sets the current stroke color to a value in the DeviceCMYK color space.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setStrokeColor(
    cyan: CGFloat,
    magenta: CGFloat,
    yellow: CGFloat,
    black: CGFloat,
    alpha: CGFloat
)
```

## Parameters 

`cyan`  

The cyan intensity value for the color to set. The DeviceCMYK color space permits the specification of a value ranging from `0.0` (does not absorb the secondary color) to `1.0` (fully absorbs the secondary color).

`magenta`  

The magenta intensity value for the color to set. The DeviceCMYK color space permits the specification of a value ranging from `0.0` (does not absorb the secondary color) to `1.0` (fully absorbs the secondary color).

`yellow`  

The yellow intensity value for the color to set. The DeviceCMYK color space permits the specification of a value ranging from `0.0` (does not absorb the secondary color) to `1.0` (fully absorbs the secondary color).

`black`  

The black intensity value for the color to set. The DeviceCMYK color space permits the specification of a value ranging from `0.0` (does not absorb the secondary color) to `1.0` (fully absorbs the secondary color).

`alpha`  

A value that specifies the opacity level. Values can range from `0.0` (transparent) to `1.0` (opaque). Values outside this range are clipped to `0.0` or `1.0`.

## Discussion

When you call this function, two things happen:

- Core Graphics sets the current stroke color space to DeviceCMYK.

- Core Graphics sets the current stroke color to the value specified by the `cyan`, `magenta`, `yellow`, `black`, and `alpha` parameters.

## See Also

### Setting Fill, Stroke, and Shadow Colors

func setFillColor(CGColor)

Sets the current fill color in a graphics context, using a CGColor.

func setFillColor(UnsafePointer&lt;CGFloat>)

Sets the current fill color.

func setFillColor(cyan: CGFloat, magenta: CGFloat, yellow: CGFloat, black: CGFloat, alpha: CGFloat)

Sets the current fill color to a value in the DeviceCMYK color space.

func setFillColor(gray: CGFloat, alpha: CGFloat)

Sets the current fill color to a value in the DeviceGray color space.

func setFillColor(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Sets the current fill color to a value in the DeviceRGB color space.

func setFillColorSpace(CGColorSpace)

Sets the fill color space in a graphics context.

func setShadow(offset: CGSize, blur: CGFloat)

Enables shadowing in a graphics context.

func setShadow(offset: CGSize, blur: CGFloat, color: CGColor?)

Enables shadowing with color a graphics context.

func setStrokeColor(CGColor)

Sets the current stroke color in a context, using a CGColor.

func setStrokeColor(UnsafePointer&lt;CGFloat>)

Sets the current stroke color.

func setStrokeColor(gray: CGFloat, alpha: CGFloat)

Sets the current stroke color to a value in the DeviceGray color space.

func setStrokeColor(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Sets the current stroke color to a value in the DeviceRGB color space.

func setStrokeColorSpace(CGColorSpace)

Sets the stroke color space in a graphics context.

func setStrokePattern(CGPattern, colorComponents: UnsafePointer&lt;CGFloat>)

Sets the stroke pattern in the specified graphics context.

func setAlpha(CGFloat)

Sets the opacity level for objects drawn in a graphics context.

