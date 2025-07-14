

- RealityKit
- Entity
-  synchronization 

Instance Property

# synchronization

The entity’s synchronization component.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var synchronization: SynchronizationComponent? { get set }
```

## Mentioned in 

Reducing CPU Utilization in Your RealityKit App

## See Also

### Synchronizing entities with other devices

var isOwner: Bool

A Boolean that indicates whether the calling process owns the entity.

func requestOwnership(timeout: TimeInterval, (SynchronizationComponent.OwnershipTransferCompletionResult) -> Void)

Requests ownership of the entity.

func withUnsynchronized(() -> Void)

Calls the given closure in a way such that component changes that the closure makes don’t trigger synchronization.

