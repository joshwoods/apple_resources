

- RealityKit
- Entity
-  requestOwnership(timeout:\_:) 

Instance Method

# requestOwnership(timeout:\_:)

Requests ownership of the entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func requestOwnership(
    timeout: TimeInterval = 15,
    _ callback: @escaping (SynchronizationComponent.OwnershipTransferCompletionResult) -> Void
)
```

## Parameters 

`timeout`  

A time in seconds to wait before giving up.

`callback`  

A closure that the method calls when the request completes or times out.

## Discussion

Requesting ownership isn’t guaranteed to succeed.

## See Also

### Synchronizing entities with other devices

var synchronization: SynchronizationComponent?

The entity’s synchronization component.

var isOwner: Bool

A Boolean that indicates whether the calling process owns the entity.

func withUnsynchronized(() -> Void)

Calls the given closure in a way such that component changes that the closure makes don’t trigger synchronization.

