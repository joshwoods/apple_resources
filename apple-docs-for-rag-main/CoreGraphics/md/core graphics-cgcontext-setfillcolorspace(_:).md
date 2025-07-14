

- Core Graphics
- CGContext
-  setFillColorSpace(\_:) 

Instance Method

# setFillColorSpace(\_:)

Sets the fill color space in a graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setFillColorSpace(_ space: CGColorSpace)
```

## Parameters 

`space`  

The new fill color space. The color space is retained; upon return, you may safely release it.

## Discussion

As a side effect of this function, Core Graphics assigns an appropriate initial value to the fill color, based on the specified color space. To change this value, call setFillColor(_:). Note that the preferred API to use is now setFillColor(_:).

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

func setStrokePattern(CGPattern, colorComponents: UnsafePointer&lt;CGFloat>)

Sets the stroke pattern in the specified graphics context.

func setAlpha(CGFloat)

Sets the opacity level for objects drawn in a graphics context.

