

- RealityKit
- Entity
-  HasSynchronization Implementations 

API Collection

# HasSynchronization Implementations

## Topics

### Instance Properties

var isOwner: Bool

A Boolean that indicates whether the calling process owns the entity.

var synchronization: SynchronizationComponent?

The entity’s synchronization component.

### Instance Methods

func requestOwnership(timeout: TimeInterval, (SynchronizationComponent.OwnershipTransferCompletionResult) -> Void)

Requests ownership of the entity.

func withUnsynchronized(() -> Void)

Calls the given closure in a way such that component changes that the closure makes don’t trigger synchronization.

