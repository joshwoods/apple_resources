

- HomeKit
-  HMCameraSnapshotControl 

Class

# HMCameraSnapshotControl

An object that can take an image snapshot from a camera.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class HMCameraSnapshotControl
```

## Topics

### Taking snapshots

func takeSnapshot()

Takes an image snapshot.

var mostRecentSnapshot: HMCameraSnapshot?

The camera’s most recent snapshot.

class HMCameraSnapshot

An object that represents a snapshot taken from a camera.

### Observing snapshot activity

var delegate: (any HMCameraSnapshotControlDelegate)?

Delegate that receives updates as the camera takes snapshots.

protocol HMCameraSnapshotControlDelegate

A set of methods used to observe the camera’s snapshot activity.

### Initializers

init()Deprecated

## Relationships

### Inherits From

- HMCameraControl

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Capturing snapshots

var snapshotControl: HMCameraSnapshotControl?

Controls the camera’s snapshot function.

