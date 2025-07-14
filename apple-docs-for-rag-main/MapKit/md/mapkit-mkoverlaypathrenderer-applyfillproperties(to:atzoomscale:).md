

- MapKit
- MKOverlayPathRenderer
-  applyFillProperties(to:atZoomScale:) 

Instance Method

# applyFillProperties(to:atZoomScale:)

Applies the receiver’s fill-related drawing properties to the specified graphics context.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
func applyFillProperties(
    to context: CGContext,
    atZoomScale zoomScale: MKZoomScale
)
```

## Parameters 

`context`  

The graphics context used to draw the view’s contents.

`zoomScale`  

The current zoom scale used for drawing.

## Discussion

This is a convenience method for applying all of the drawing properties used when filling a path. This method applies the current fill color to the specified graphics context.

## See Also

### Drawing the path

func applyStrokeProperties(to: CGContext, atZoomScale: MKZoomScale)

Applies the renderer’s stroke-related drawing properties to the specified graphics context.

func strokePath(CGPath, in: CGContext)

Draws a line along the specified path.

func fillPath(CGPath, in: CGContext)

Fills the area that the specified path encloses.

var shouldRasterize: Bool

A Boolean value that determines whether the overlay path renderer renders the overlay as a bitmap before compositing.

