

- MapKit
-  MKMapItemRequest 

Class

# MKMapItemRequest

A utility class you use to request additional information about a map feature.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 15.0+tvOS 18.0+visionOS 1.0+

``` source
class MKMapItemRequest
```

## Mentioned in 

Identifying unique locations with Place IDs

## Topics

### Creating a request

convenience init(feature: MapFeature)

Creates a new map item request with the specified map feature.

init(mapItemIdentifier: MKMapItem.Identifier)

Create a request with a map item identifier.

init(mapFeatureAnnotation: MKMapFeatureAnnotation)

Creates a new map item request with the specified feature annotation.

### Configuring the item request

var mapFeature: MapFeature?

The map feature.

var mapFeatureAnnotation: MKMapFeatureAnnotation?

The feature annotation.

var mapItemIdentifier: MKMapItem.Identifier?

The map item identifer.

var feature: MapFeature

The map feature.

Deprecated

var featureAnnotation: MKMapFeatureAnnotation

The feature annotation.

Deprecated

### Starting and stopping requests

func cancel()

Cancels an in-progress map item request.

func getMapItem(completionHandler: (MKMapItem?, (any Error)?) -> Void)

Requests a map item and calls the provided completion handler.

### Checking the status of a request

var isCancelled: Bool

A Boolean value that indicates if the cancellation of the request was successful.

var isLoading: Bool

A Boolean value that indicates if the request is loading.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Points of interest

Identifying unique locations with Place IDs

Obtain information about a point of interest that persists over its lifetime.

class MKMapFeatureAnnotation

A class that describes an annotation element on the map’s display such as a point of interest, territorial boundary, or physical feature.

struct MKMapFeatureOptions

A structure you use to tell the map which kinds of features users can interact with.

class MKIconStyle

A class you use to customize the annotation view icon of a point of interest (POI) on the map.

class MKPointOfInterestFilter

A filter that includes or excludes point of interest categories from a map view, local search, or local search completer.

struct MKPointOfInterestCategory

A point of interest category.

