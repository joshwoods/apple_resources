

- UIKit
-  UIRectFrameUsingBlendMode(\_:\_:) 

Function

# UIRectFrameUsingBlendMode(\_:\_:)

Draws a frame around the inside of a rectangle using the specified blend mode.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
func UIRectFrameUsingBlendMode(
    _ rect: CGRect,
    _ blendMode: CGBlendMode
)
```

## Parameters 

`rect`  

The rectangle defining the area in which to draw.

`blendMode`  

The blend mode to use during drawing.

## Discussion

This function draws a frame around the inside of rect in the fill color of the current graphics context and using the specified blend mode. The width is equal to 1.0 in the current coordinate system. Since the frame is drawn inside the rectangle, it’s visible even if drawing is clipped to the rectangle. If the current graphics context is `nil`, this function does nothing.

Because this function doesn’t draw directly on the line, but rather inside it, it uses the current fill color (not stroke color) when drawing.

This function may be called from any thread of your app.

## See Also

### Paths

class UIBezierPath

A path that consists of straight and curved line segments that you can render in your custom views.

func UIRectFill(CGRect)

Fills the specified rectangle with the current color.

func UIRectFillUsingBlendMode(CGRect, CGBlendMode)

Fills a rectangle with the current fill color using the specified blend mode.

func UIRectFrame(CGRect)

Draws a frame around the inside of the specified rectangle.

