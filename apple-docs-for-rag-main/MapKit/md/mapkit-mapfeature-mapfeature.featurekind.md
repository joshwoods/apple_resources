

- MapKit
- MapFeature
-  MapFeature.FeatureKind 

Structure

# MapFeature.FeatureKind

The kind of feature represented by a map feature.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct FeatureKind
```

## Topics

### Kinds of features

static var physicalFeature: MapFeature.FeatureKind

A physical map feature.

static var pointOfInterest: MapFeature.FeatureKind

A point of interest.

static var territory: MapFeature.FeatureKind

A territory or political boundary.

## Relationships

### Conforms To

- Copyable
- Equatable

## See Also

### Accessing the feature’s properties

var kind: MapFeature.FeatureKind

The kind of feature represented by the map feature.

var coordinate: CLLocationCoordinate2D

The coordinate of the map feature.

var title: String?

The title of the map feature.

var backgroundColor: Color?

The background color associated with the map feature.

var image: Image?

An image associated with the map feature.

var pointOfInterestCategory: MKPointOfInterestCategory?

The point of interest category of the map feature.

