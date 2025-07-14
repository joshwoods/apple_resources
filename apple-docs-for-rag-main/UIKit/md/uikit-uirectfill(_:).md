

- UIKit
-  UIRectFill(\_:) 

Function

# UIRectFill(\_:)

Fills the specified rectangle with the current color.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
func UIRectFill(_ rect: CGRect)
```

## Parameters 

`rect`  

The rectangle defining the area in which to draw.

## Discussion

Fills the specified rectangle using the fill color of the current graphics context and the `kCGBlendModeCopy` blend mode.

This function may be called from any thread of your app.

## See Also

### Paths

class UIBezierPath

A path that consists of straight and curved line segments that you can render in your custom views.

func UIRectFillUsingBlendMode(CGRect, CGBlendMode)

Fills a rectangle with the current fill color using the specified blend mode.

func UIRectFrame(CGRect)

Draws a frame around the inside of the specified rectangle.

func UIRectFrameUsingBlendMode(CGRect, CGBlendMode)

Draws a frame around the inside of a rectangle using the specified blend mode.

