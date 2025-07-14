

- UIKit
-  UIRectFrame(\_:) 

Function

# UIRectFrame(\_:)

Draws a frame around the inside of the specified rectangle.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
func UIRectFrame(_ rect: CGRect)
```

## Parameters 

`rect`  

The rectangle defining the area in which to draw.

## Discussion

This function draws a frame around the inside of `rect` in the stroke color of the current graphics context and using the `kCGBlendModeCopy` blend mode. The width is equal to 1.0 in the current coordinate system. Because the frame is drawn inside the rectangle, it is visible even if drawing is clipped to the rectangle. If the current graphics context is `nil`, this function does nothing.

This function may be called from any thread of your app.

## See Also

### Paths

class UIBezierPath

A path that consists of straight and curved line segments that you can render in your custom views.

func UIRectFill(CGRect)

Fills the specified rectangle with the current color.

func UIRectFillUsingBlendMode(CGRect, CGBlendMode)

Fills a rectangle with the current fill color using the specified blend mode.

func UIRectFrameUsingBlendMode(CGRect, CGBlendMode)

Draws a frame around the inside of a rectangle using the specified blend mode.

