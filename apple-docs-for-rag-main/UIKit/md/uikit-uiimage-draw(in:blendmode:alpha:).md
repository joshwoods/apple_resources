

- UIKit
- UIImage
-  draw(in:blendMode:alpha:) 

Instance Method

# draw(in:blendMode:alpha:)

Draws the entire image in the specified rectangle using the specified compositing options.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func draw(
    in rect: CGRect,
    blendMode: CGBlendMode,
    alpha: CGFloat
)
```

## Parameters 

`rect`  

The rectangle (in the coordinate system of the graphics context) in which to draw the image.

`blendMode`  

The blend mode to use when compositing the image.

`alpha`  

The desired opacity of the image, specified as a value between 0.0 and 1.0. A value of 0.0 renders the image totally transparent while 1.0 renders it fully opaque. Values larger than 1.0 are interpreted as 1.0.

## Discussion

This method scales the image as needed to make it fit in the specified rectangle. This method draws the image in the current graphics context, respecting the image’s orientation setting. In the default coordinate system, images are situated down and to the right of the origin of the specified rectangle. This method respects any transforms applied to the current graphics context, however.

## See Also

### Drawing images

func draw(at: CGPoint)

Draws the image at the specified point in the current context.

func draw(at: CGPoint, blendMode: CGBlendMode, alpha: CGFloat)

Draws the entire image at the specified point using the custom compositing options.

func draw(in: CGRect)

Draws the entire image in the specified rectangle, scaling it as necessary to fit.

func drawAsPattern(in: CGRect)

Draws a tiled Quartz pattern using the receiver’s contents as the tile pattern.

