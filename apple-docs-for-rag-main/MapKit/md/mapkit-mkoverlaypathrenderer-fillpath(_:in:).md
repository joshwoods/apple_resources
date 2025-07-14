

- MapKit
- MKOverlayPathRenderer
-  fillPath(\_:in:) 

Instance Method

# fillPath(\_:in:)

Fills the area that the specified path encloses.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
func fillPath(
    _ path: CGPath,
    in context: CGContext
)
```

## Parameters 

`path`  

The path to fill.

`context`  

The graphics context in which to draw the path.

## Discussion

You must set the current fill color before calling this method. Typically you do this by calling the applyFillProperties(to:atZoomScale:) method prior to drawing. If the fillColor property is currently `nil`, this method does nothing.

## See Also

### Drawing the path

func applyStrokeProperties(to: CGContext, atZoomScale: MKZoomScale)

Applies the renderer’s stroke-related drawing properties to the specified graphics context.

func applyFillProperties(to: CGContext, atZoomScale: MKZoomScale)

Applies the receiver’s fill-related drawing properties to the specified graphics context.

func strokePath(CGPath, in: CGContext)

Draws a line along the specified path.

var shouldRasterize: Bool

A Boolean value that determines whether the overlay path renderer renders the overlay as a bitmap before compositing.

