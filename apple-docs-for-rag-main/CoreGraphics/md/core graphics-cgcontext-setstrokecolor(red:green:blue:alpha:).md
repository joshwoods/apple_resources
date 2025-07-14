

- Core Graphics
- CGContext
-  setStrokeColor(red:green:blue:alpha:) 

Instance Method

# setStrokeColor(red:green:blue:alpha:)

Sets the current stroke color to a value in the DeviceRGB color space.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setStrokeColor(
    red: CGFloat,
    green: CGFloat,
    blue: CGFloat,
    alpha: CGFloat
)
```

## Parameters 

`red`  

The red intensity value for the color to set. The DeviceRGB color space permits the specification of a value ranging from `0.0` (zero intensity) to `1.0` (full intensity).

`green`  

The green intensity value for the color to set. The DeviceRGB color space permits the specification of a value ranging from `0.0` (zero intensity) to `1.0` (full intensity).

`blue`  

The blue intensity value for the color to set. The DeviceRGB color space permits the specification of a value ranging from `0.0` (zero intensity) to `1.0` (full intensity).

`alpha`  

A value that specifies the opacity level. Values can range from `0.0` (transparent) to `1.0` (opaque). Values outside this range are clipped to `0.0` or `1.0`.

## Discussion

When you call this function, two things happen:

- Core Graphics sets the current stroke color space to DeviceRGB.

- Core Graphics sets the current stroke color to the value specified by the `red`, `green`, `blue`, and `alpha` parameters.

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

func setStrokeColor(cyan: CGFloat, magenta: CGFloat, yellow: CGFloat, black: CGFloat, alpha: CGFloat)

Sets the current stroke color to a value in the DeviceCMYK color space.

func setStrokeColor(gray: CGFloat, alpha: CGFloat)

Sets the current stroke color to a value in the DeviceGray color space.

func setStrokeColorSpace(CGColorSpace)

Sets the stroke color space in a graphics context.

func setStrokePattern(CGPattern, colorComponents: UnsafePointer&lt;CGFloat>)

Sets the stroke pattern in the specified graphics context.

func setAlpha(CGFloat)

Sets the opacity level for objects drawn in a graphics context.

