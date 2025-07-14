

- MapKit
- MKOverlayRenderer
-  blendMode 

Instance Property

# blendMode

The blend mode to apply to the overlay.

iOS 16.0+iPadOS 16.0+tvOS 16.0+visionOS 1.0+

``` source
var blendMode: CGBlendMode { get set }
```

## Discussion

Choose the blend mode from one of the possible CGBlendMode enumerations.

## See Also

### Attributes of the overlay

var overlay: any MKOverlay

The overlay object containing the data for drawing.

var alpha: CGFloat

The amount of transparency to apply to the overlay.

var contentScaleFactor: CGFloat

The scale factor for drawing the overlay’s content.

