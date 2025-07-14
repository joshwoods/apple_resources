

- RealityKit
- Entity
-  isOwner 

Instance Property

# isOwner

A Boolean that indicates whether the calling process owns the entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var isOwner: Bool { get }
```

## Discussion

The calling process owns the entity if the value is `true`.

## See Also

### Synchronizing entities with other devices

var synchronization: SynchronizationComponent?

The entity’s synchronization component.

func requestOwnership(timeout: TimeInterval, (SynchronizationComponent.OwnershipTransferCompletionResult) -> Void)

Requests ownership of the entity.

func withUnsynchronized(() -> Void)

Calls the given closure in a way such that component changes that the closure makes don’t trigger synchronization.

