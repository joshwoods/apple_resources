

- HomeKit
- HMCameraSnapshotControlDelegate
-  cameraSnapshotControlDidUpdateMostRecentSnapshot(\_:) 

Instance Method

# cameraSnapshotControlDidUpdateMostRecentSnapshot(\_:)

Tells the delegate that the most recent snapshot has been updated.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
optional func cameraSnapshotControlDidUpdateMostRecentSnapshot(_ cameraSnapshotControl: HMCameraSnapshotControl)
```

## Parameters 

`cameraSnapshotControl`  

The camera snapshot control responsible for the updated snapshot.

## See Also

### Observing snapshot activity

func cameraSnapshotControl(HMCameraSnapshotControl, didTake: HMCameraSnapshot?, error: (any Error)?)

Tells the delegate that the camera has taken a new snapshot.

