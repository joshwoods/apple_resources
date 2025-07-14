

- MapKit
- MKOverlayRenderer
-  overlay 

Instance Property

# overlay

The overlay object containing the data for drawing.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var overlay: any MKOverlay { get }
```

## Discussion

The overlay object contains the coordinate at which to draw the overlay and other information that your app provides.

## See Also

### Attributes of the overlay

var alpha: CGFloat

The amount of transparency to apply to the overlay.

var contentScaleFactor: CGFloat

The scale factor for drawing the overlay’s content.

var blendMode: CGBlendMode

The blend mode to apply to the overlay.

