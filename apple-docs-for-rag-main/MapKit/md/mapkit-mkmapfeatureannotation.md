

- MapKit
-  MKMapFeatureAnnotation 

Class

# MKMapFeatureAnnotation

A class that describes an annotation element on the map’s display such as a point of interest, territorial boundary, or physical feature.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class MKMapFeatureAnnotation
```

## Topics

### Customizing the annotation

var featureType: MKMapFeatureAnnotation.FeatureType

The type of map feature this annotation represents.

enum FeatureType

Values that describe the kinds of features visible on the map.

var iconStyle: MKIconStyle?

The icon style of a feature annotation.

var pointOfInterestCategory: MKPointOfInterestCategory?

The feature annotation’s point of interest category.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MKAnnotation
- NSObjectProtocol

## See Also

### Points of interest

Identifying unique locations with Place IDs

Obtain information about a point of interest that persists over its lifetime.

struct MKMapFeatureOptions

A structure you use to tell the map which kinds of features users can interact with.

class MKMapItemRequest

A utility class you use to request additional information about a map feature.

class MKIconStyle

A class you use to customize the annotation view icon of a point of interest (POI) on the map.

class MKPointOfInterestFilter

A filter that includes or excludes point of interest categories from a map view, local search, or local search completer.

struct MKPointOfInterestCategory

A point of interest category.

