

- RealityKit
- SynchronizationEvents
-  SynchronizationEvents.OwnershipRequest 

Structure

# SynchronizationEvents.OwnershipRequest

The event raised when a network peer wants to gain ownership of an entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct OwnershipRequest
```

## Topics

### Getting the involved parties

let entity: Entity

The entity over which the network peer would like to gain ownership.

let requester: any SynchronizationPeerID

The network peer requesting ownership.

### Accepting the request

let accept: () -> Void

The callback function that the current owner calls to grant ownership to the requesting peer.

## Relationships

### Conforms To

- Event
- Sendable

## See Also

### Detecting ownership updates

struct OwnershipChanged

The event raised when ownership of an entity changes.

