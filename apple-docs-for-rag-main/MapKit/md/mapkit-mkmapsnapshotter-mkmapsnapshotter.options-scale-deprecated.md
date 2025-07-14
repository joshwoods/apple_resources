

- MapKit
- MKMapSnapshotter
- MKMapSnapshotter.Options
-  scale Deprecated

Instance Property

# scale

The scale factor to use when creating the image.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1+tvOS 9.2+visionOS 1.0–2.4Deprecated

``` source
var scale: CGFloat { get set }
```

Deprecated

Use traitCollection instead.

## Discussion

The value of this property is either `1.0` or `2.0`, depending on whether the device has a standard or Retina display. Set the value to `1.0` if you want to display the resulting image on a standard resolution display. Set the value to 2.0 if you want to display the image on a Retina display or want to use the image for printing.

This snapshotter sets this property to a default value that corresponds to the resolution of the current device’s display. You can change the value as needed to generate an image suitable for display on a different device.

## See Also

### Configuring the image output

var traitCollection: UITraitCollection

Traits that determine the appearance of the map snapshot.

var size: CGSize

The size of the image that you want to create.

var appearance: NSAppearance?

The visual style (light or dark) to apply to the map when rendering the snapshot image.

