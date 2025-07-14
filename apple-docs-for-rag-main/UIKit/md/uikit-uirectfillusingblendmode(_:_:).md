

- UIKit
-  UIRectFillUsingBlendMode(\_:\_:) 

Function

# UIRectFillUsingBlendMode(\_:\_:)

Fills a rectangle with the current fill color using the specified blend mode.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
func UIRectFillUsingBlendMode(
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

This function draws the rectangle in the current graphics context. If the current graphics context is `nil`, this function does nothing.

This function may be called from any thread of your app.

## See Also

### Paths

class UIBezierPath

A path that consists of straight and curved line segments that you can render in your custom views.

func UIRectFill(CGRect)

Fills the specified rectangle with the current color.

func UIRectFrame(CGRect)

Draws a frame around the inside of the specified rectangle.

func UIRectFrameUsingBlendMode(CGRect, CGBlendMode)

Draws a frame around the inside of a rectangle using the specified blend mode.

