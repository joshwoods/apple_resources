

- MapKit
- MKOverlayRenderer
-  alpha 

Instance Property

# alpha

The amount of transparency to apply to the overlay.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var alpha: CGFloat { get set }
```

## Discussion

The value in this property can be in the range `0.0` to `1.0`, where `0.0` represents total transparency and `1.0` represents total opacity. The default value of this property is `1.0`.

## See Also

### Attributes of the overlay

var overlay: any MKOverlay

The overlay object containing the data for drawing.

var contentScaleFactor: CGFloat

The scale factor for drawing the overlay’s content.

var blendMode: CGBlendMode

The blend mode to apply to the overlay.

