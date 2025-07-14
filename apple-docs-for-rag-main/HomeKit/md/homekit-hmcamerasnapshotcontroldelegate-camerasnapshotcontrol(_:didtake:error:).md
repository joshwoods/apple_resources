

- HomeKit
- HMCameraSnapshotControlDelegate
-  cameraSnapshotControl(\_:didTake:error:) 

Instance Method

# cameraSnapshotControl(\_:didTake:error:)

Tells the delegate that the camera has taken a new snapshot.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
optional func cameraSnapshotControl(
    _ cameraSnapshotControl: HMCameraSnapshotControl,
    didTake snapshot: HMCameraSnapshot?,
    error: (any Error)?
)
```

## Parameters 

`cameraSnapshotControl`  

The camera snapshot control responsible for the new snapshot.

`snapshot`  

The snapshot taken by the camera. `nil` if there was a problem.

`error`  

An error that is populated if there was a problem taking the snapshot; `nil` otherwise.

## See Also

### Observing snapshot activity

func cameraSnapshotControlDidUpdateMostRecentSnapshot(HMCameraSnapshotControl)

Tells the delegate that the most recent snapshot has been updated.

