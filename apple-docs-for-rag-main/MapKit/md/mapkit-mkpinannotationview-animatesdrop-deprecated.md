

- MapKit
- MKPinAnnotationView
-  animatesDrop Deprecated

Instance Property

# animatesDrop

A Boolean value indicating whether the annotation view is animated onto the screen.

iOS 3.0–16.0DeprecatediPadOS 3.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.9–13.0DeprecatedtvOS 9.2–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var animatesDrop: Bool { get set }
```

## Discussion

When this property is true, the map view animates the appearance of pin annotation views by making them appear to drop onto the map at the target point. This animation occurs whenever the view transitions from offscreen to onscreen.

## See Also

### Getting and Setting Attributes

var pinTintColor: UIColor!

The color of the pin head.

Deprecated

var pinColor: MKPinAnnotationColor

The color of the pin head.

Deprecated

