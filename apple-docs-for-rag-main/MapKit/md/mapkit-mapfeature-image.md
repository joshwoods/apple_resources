

- MapKit
- MapFeature
-  image 

Instance Property

# image

An image associated with the map feature.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
var image: Image? { get }
```

## Discussion

If this feature doesn’t have an associated image, this property is `nil`.

## See Also

### Accessing the feature’s properties

var kind: MapFeature.FeatureKind

The kind of feature represented by the map feature.

struct FeatureKind

The kind of feature represented by a map feature.

var coordinate: CLLocationCoordinate2D

The coordinate of the map feature.

var title: String?

The title of the map feature.

var backgroundColor: Color?

The background color associated with the map feature.

var pointOfInterestCategory: MKPointOfInterestCategory?

The point of interest category of the map feature.

