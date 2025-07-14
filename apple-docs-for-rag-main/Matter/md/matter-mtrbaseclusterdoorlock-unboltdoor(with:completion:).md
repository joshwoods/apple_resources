

- Matter
- MTRBaseClusterDoorLock
-  unboltDoor(with:completion:) 

Instance Method

# unboltDoor(with:completion:)

Command UnboltDoor

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func unboltDoor(
    with params: MTRDoorLockClusterUnboltDoorParams?,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func unboltDoor(with params: MTRDoorLockClusterUnboltDoorParams?) async throws
```

## Discussion

This command causes the lock device to unlock the door without pulling the latch.

