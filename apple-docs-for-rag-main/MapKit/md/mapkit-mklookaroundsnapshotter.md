

- MapKit
-  MKLookAroundSnapshotter 

Class

# MKLookAroundSnapshotter

A utility class that you use to create a static image from a LookAround scene.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class MKLookAroundSnapshotter
```

## Topics

### Creating a snapshotter object

init(scene: MKLookAroundScene, options: MKLookAroundSnapshotter.Options)

Create a new snapshotter object with the scene and options you specify.

### Starting and stopping a snapshot

func cancel()

Cancels an in-progress snapshot request.

func getSnapshotWithCompletionHandler((MKLookAroundSnapshotter.Snapshot?, (any Error)?) -> Void)

Requests a new snapshot and calls the completion handler you provide.

### Monitoring the progress of a snaphot

var isLoading: Bool

A Boolean value that indicates whether the snapshot request is loading.

### Customizing the snapshot

class Options

Values you use to customize LookAround snapshots.

### Accessing snapshot imagery

class Snapshot

An object that contains a snapshot image.

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

class MKLookAroundSceneRequest

A class you use to request a LookAround scene at the location you specify.

class MKLookAroundViewController

A class that manages the presentation and display of a LookAround view.

