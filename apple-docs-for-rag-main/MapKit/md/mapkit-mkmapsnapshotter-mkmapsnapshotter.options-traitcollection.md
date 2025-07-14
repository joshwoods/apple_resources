

- MapKit
- MKMapSnapshotter
- MKMapSnapshotter.Options
-  traitCollection 

Instance Property

# traitCollection

Traits that determine the appearance of the map snapshot.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying
var traitCollection: UITraitCollection { get set }
```

## See Also

### Configuring the image output

var size: CGSize

The size of the image that you want to create.

var appearance: NSAppearance?

The visual style (light or dark) to apply to the map when rendering the snapshot image.

var scale: CGFloat

The scale factor to use when creating the image.

Deprecated

