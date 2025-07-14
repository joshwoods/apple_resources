

- MapKit
-  MKPointOfInterestFilter 

Class

# MKPointOfInterestFilter

A filter that includes or excludes point of interest categories from a map view, local search, or local search completer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MKPointOfInterestFilter
```

## Overview

You can apply a point of interest filter in a map view (pointOfInterestFilter), a local search request (pointOfInterestFilter), a search completer (pointOfInterestFilter), and in snapshot options (pointOfInterestFilter).

## Topics

### Creating filters

class var excludingAll: MKPointOfInterestFilter

A filter that excludes all point of interest categories.

class var includingAll: MKPointOfInterestFilter

A filter that includes all point of interest categories.

init(excluding: [MKPointOfInterestCategory])

Initialize the point of interest filter with a list of categories to exclude.

init(including: [MKPointOfInterestCategory])

Initialize the point of interest filter with a list of categories to include.

### Querying filter behavior

func excludes(MKPointOfInterestCategory) -> Bool

Returns a Boolean value indicating whether the filter excludes the point of interest category.

func includes(MKPointOfInterestCategory) -> Bool

Returns a Boolean value indicating whether the filter includes the point of interest category.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Points of interest

Identifying unique locations with Place IDs

Obtain information about a point of interest that persists over its lifetime.

class MKMapFeatureAnnotation

A class that describes an annotation element on the map’s display such as a point of interest, territorial boundary, or physical feature.

struct MKMapFeatureOptions

A structure you use to tell the map which kinds of features users can interact with.

class MKMapItemRequest

A utility class you use to request additional information about a map feature.

class MKIconStyle

A class you use to customize the annotation view icon of a point of interest (POI) on the map.

struct MKPointOfInterestCategory

A point of interest category.

