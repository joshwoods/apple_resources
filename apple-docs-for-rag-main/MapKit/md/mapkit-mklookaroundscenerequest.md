

- MapKit
-  MKLookAroundSceneRequest 

Class

# MKLookAroundSceneRequest

A class you use to request a LookAround scene at the location you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class MKLookAroundSceneRequest
```

## Topics

### Creating a LookAround scene

init(coordinate: CLLocationCoordinate2D)

Creates a LookAround scene at the specified coordinates.

init(mapItem: MKMapItem)

Creates a LookAround scene with the location described by the specified map item.

### Specifying the request’s location

var coordinate: CLLocationCoordinate2D

A coordinate value that describes the location of the LookAround scene.

var mapItem: MKMapItem?

A map item that describes the location of the LookAround scene.

### Starting and stopping scene requests

func cancel()

Cancels the pending scene request.

func getSceneWithCompletionHandler((MKLookAroundScene?, (any Error)?) -> Void)

Requests a LookAround scene and calls the specified completion handler.

### Monitoring the progress of scene requests

var isCancelled: Bool

A Boolean value that indicates if the cancellation of a scene request was successful.

var isLoading: Bool

A Boolean value that indicates whether a scene request is loading.

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

### Exploring at street level

class MKLookAroundScene

A utility class that encapsulates information the framework requires to retrieve and display a specific Look Around location’s imagery.

class MKLookAroundViewController

A class that manages the presentation and display of a LookAround view.

class MKLookAroundSnapshotter

A utility class that you use to create a static image from a LookAround scene.

