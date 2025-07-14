

- MapKit
-  MKMapFeatureOptions 

Structure

# MKMapFeatureOptions

A structure you use to tell the map which kinds of features users can interact with.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
struct MKMapFeatureOptions
```

## Topics

### Initializers

init(rawValue: Int)

Creates a new feature option structure with the specified value.

### Selecting interactive map features

static var physicalFeatures: MKMapFeatureOptions

The option that represents physical map features such as mountain ranges, rivers, and ocean basins.

static var pointsOfInterest: MKMapFeatureOptions

The option that represents points of interest such as museums, cafes, parks, or schools.

static var territories: MKMapFeatureOptions

The option that represents territorial boundaries such as a national border, a state boundary, or a neighborhood.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Points of interest

Identifying unique locations with Place IDs

Obtain information about a point of interest that persists over its lifetime.

class MKMapFeatureAnnotation

A class that describes an annotation element on the map’s display such as a point of interest, territorial boundary, or physical feature.

class MKMapItemRequest

A utility class you use to request additional information about a map feature.

class MKIconStyle

A class you use to customize the annotation view icon of a point of interest (POI) on the map.

class MKPointOfInterestFilter

A filter that includes or excludes point of interest categories from a map view, local search, or local search completer.

struct MKPointOfInterestCategory

A point of interest category.

