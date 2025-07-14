

- MapKit
- MKOverlayPathRenderer
-  shouldRasterize 

Instance Property

# shouldRasterize

A Boolean value that determines whether the overlay path renderer renders the overlay as a bitmap before compositing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var shouldRasterize: Bool { get set }
```

## Discussion

The default value is `false`.

Whenever possible, MapKit vectorizes overlay shapes by default so that they scale along with the map and remain sharp. In some cases, you may want to force the rasterization of an overlay and not vectorize it. Set this variable to `true` to force the overlay path renderer to render the overlay as a bitmap.

## See Also

### Drawing the path

func applyStrokeProperties(to: CGContext, atZoomScale: MKZoomScale)

Applies the renderer’s stroke-related drawing properties to the specified graphics context.

func applyFillProperties(to: CGContext, atZoomScale: MKZoomScale)

Applies the receiver’s fill-related drawing properties to the specified graphics context.

func strokePath(CGPath, in: CGContext)

Draws a line along the specified path.

func fillPath(CGPath, in: CGContext)

Fills the area that the specified path encloses.

