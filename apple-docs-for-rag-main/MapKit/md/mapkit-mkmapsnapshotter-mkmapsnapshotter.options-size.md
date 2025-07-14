

- MapKit
- MKMapSnapshotter
- MKMapSnapshotter.Options
-  size 

Instance Property

# size

The size of the image that you want to create.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

**macOS**

``` source
var size: NSSize { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
var size: CGSize { get set }
```

## Discussion

The default value of this property is 256 by 256 points.

## See Also

### Configuring the image output

var traitCollection: UITraitCollection

Traits that determine the appearance of the map snapshot.

var appearance: NSAppearance?

The visual style (light or dark) to apply to the map when rendering the snapshot image.

var scale: CGFloat

The scale factor to use when creating the image.

Deprecated

