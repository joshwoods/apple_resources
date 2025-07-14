

- HomeKit
- HMCameraSnapshotControl
-  delegate 

Instance Property

# delegate

Delegate that receives updates as the camera takes snapshots.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
weak var delegate: (any HMCameraSnapshotControlDelegate)? { get set }
```

## See Also

### Observing snapshot activity

protocol HMCameraSnapshotControlDelegate

A set of methods used to observe the camera’s snapshot activity.

