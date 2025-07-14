

- MapKit
- MKPinAnnotationView
-  pinColor Deprecated

Instance Property

# pinColor

The color of the pin head.

iOS 3.0–9.0DeprecatediPadOS 3.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.11Deprecated

``` source
@MainActor
var pinColor: MKPinAnnotationColor { get set }
```

Deprecated

Use pinTintColor instead.

## Discussion

The Maps application uses different pin colors for different types of map annotations. Your own map annotation should use the available pin colors in the same way. For a description of when to use each type of pin, see the constants of MKPinAnnotationColor.

## See Also

### Getting and Setting Attributes

var pinTintColor: UIColor!

The color of the pin head.

Deprecated

var animatesDrop: Bool

A Boolean value indicating whether the annotation view is animated onto the screen.

Deprecated

