

- Core Graphics
- CGContext
-  setShadow(offset:blur:) 

Instance Method

# setShadow(offset:blur:)

Enables shadowing in a graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setShadow(
    offset: CGSize,
    blur: CGFloat
)
```

## Parameters 

`offset`  

Specifies a translation of the context’s coordinate system, to establish an offset for the shadow (`{0,0}` specifies a light source immediately above the screen).

`blur`  

A non-negative number specifying the amount of blur.

## Discussion

Shadow parameters are part of the graphics state in a context. After shadowing is set, all objects drawn are shadowed using a black color with 1/3 alpha (in effect, RGBA = `{0, 0, 0, 1.0/3.0}`) in the DeviceRGB color space.

To turn off shadowing:

- Use the standard save/restore mechanism for the graphics state.

- Use setShadow(offset:blur:color:) to set the shadow color to a fully transparent color (or pass `NULL` as the color).

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

func setStrokePattern(CGPattern, colorComponents: UnsafePointer&lt;CGFloat>)

Sets the stroke pattern in the specified graphics context.

func setAlpha(CGFloat)

Sets the opacity level for objects drawn in a graphics context.

