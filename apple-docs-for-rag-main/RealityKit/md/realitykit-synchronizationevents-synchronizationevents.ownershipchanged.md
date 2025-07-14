

- RealityKit
- SynchronizationEvents
-  SynchronizationEvents.OwnershipChanged 

Structure

# SynchronizationEvents.OwnershipChanged

The event raised when ownership of an entity changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct OwnershipChanged
```

## Topics

### Getting the involved parties

let entity: Entity

The entity for which ownership is changed.

let newOwner: (any SynchronizationPeerID)?

The new owner of the entity.

## Relationships

### Conforms To

- Event
- Sendable

## See Also

### Detecting ownership updates

struct OwnershipRequest

The event raised when a network peer wants to gain ownership of an entity.

