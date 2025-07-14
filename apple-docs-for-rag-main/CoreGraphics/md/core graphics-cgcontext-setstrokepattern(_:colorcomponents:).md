

- Core Graphics
- CGContext
-  setStrokePattern(\_:colorComponents:) 

Instance Method

# setStrokePattern(\_:colorComponents:)

Sets the stroke pattern in the specified graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setStrokePattern(
    _ pattern: CGPattern,
    colorComponents components: UnsafePointer
)
```

## Parameters 

`pattern`  

A pattern for stroking. In Objective-C, the object is retained; upon return, you may safely release it.

`components`  

If the specified pattern is an uncolored (or masking) pattern, pass an array of intensity values that specify the color to use when the pattern is painted. The number of array elements must equal the number of components in the base space of the stroke pattern color space, plus an additional component for the alpha value.

If the specified pattern is a color pattern, pass an alpha value.

## Discussion

The current stroke color space must be a pattern color space. Otherwise, the result of calling this function is undefined. If you want to set a stroke color, not a stroke pattern, use setStrokeColor(_:).

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

func setStrokeColor(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Sets the current stroke color to a value in the DeviceRGB color space.

func setStrokeColorSpace(CGColorSpace)

Sets the stroke color space in a graphics context.

func setAlpha(CGFloat)

Sets the opacity level for objects drawn in a graphics context.

