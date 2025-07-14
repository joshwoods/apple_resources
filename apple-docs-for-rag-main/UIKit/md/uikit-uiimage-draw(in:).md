

- UIKit
- UIImage
-  draw(in:) 

Instance Method

# draw(in:)

Draws the entire image in the specified rectangle, scaling it as necessary to fit.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func draw(in rect: CGRect)
```

## Parameters 

`rect`  

The rectangle (in the coordinate system of the graphics context) in which to draw the image.

## Discussion

This method draws the entire image in the current graphics context, respecting the image’s orientation setting. In the default coordinate system, images are situated down and to the right of the origin of the specified rectangle. This method respects any transforms applied to the current graphics context, however.

This method draws the image at full opacity using the CGBlendMode.normal blend mode.

## See Also

### Drawing images

func draw(at: CGPoint)

Draws the image at the specified point in the current context.

func draw(at: CGPoint, blendMode: CGBlendMode, alpha: CGFloat)

Draws the entire image at the specified point using the custom compositing options.

func draw(in: CGRect, blendMode: CGBlendMode, alpha: CGFloat)

Draws the entire image in the specified rectangle using the specified compositing options.

func drawAsPattern(in: CGRect)

Draws a tiled Quartz pattern using the receiver’s contents as the tile pattern.

