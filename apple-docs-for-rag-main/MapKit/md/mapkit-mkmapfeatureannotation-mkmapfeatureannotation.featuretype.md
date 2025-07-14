

- MapKit
- MKMapFeatureAnnotation
-  MKMapFeatureAnnotation.FeatureType 

Enumeration

# MKMapFeatureAnnotation.FeatureType

Values that describe the kinds of features visible on the map.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
enum FeatureType
```

## Topics

### Kinds of annotations

case physicalFeature

A physical feature on the Earth such as a mountain range, river, or ocean basin.

case pointOfInterest

A point of interest, such as a museum, cafe, park, or school.

case territory

A territorial or regional boundary, such as a national border, a state boundary, or a neighborhood.

case physicalFeature

A physical feature on the Earth such as a mountain range, river, or ocean basin.

case pointOfInterest

A point of interest, such as a museum, cafe, park, or school.

case territory

A territorial or regional boundary, such as a national border, a state boundary, or a neighborhood.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Customizing the annotation

var featureType: MKMapFeatureAnnotation.FeatureType

The type of map feature this annotation represents.

var iconStyle: MKIconStyle?

The icon style of a feature annotation.

var pointOfInterestCategory: MKPointOfInterestCategory?

The feature annotation’s point of interest category.

