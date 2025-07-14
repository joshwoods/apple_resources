

- HomeKit
-  HMCameraSnapshotControlDelegate 

Protocol

# HMCameraSnapshotControlDelegate

A set of methods used to observe the camera’s snapshot activity.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
protocol HMCameraSnapshotControlDelegate : NSObjectProtocol
```

## Topics

### Observing snapshot activity

func cameraSnapshotControl(HMCameraSnapshotControl, didTake: HMCameraSnapshot?, error: (any Error)?)

Tells the delegate that the camera has taken a new snapshot.

func cameraSnapshotControlDidUpdateMostRecentSnapshot(HMCameraSnapshotControl)

Tells the delegate that the most recent snapshot has been updated.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Observing snapshot activity

var delegate: (any HMCameraSnapshotControlDelegate)?

Delegate that receives updates as the camera takes snapshots.

