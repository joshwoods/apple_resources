

- RealityKit
-  SynchronizationService 

Protocol

# SynchronizationService

An interface that enables entity synchronization among a group of local peers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
protocol SynchronizationService : AnyObject
```

## Topics

### Managing ownership

func owner(of: Entity) -> (any SynchronizationPeerID)?

Gets the device that owns a given entity, if any.

**Required**

func giveOwnership(of: Entity, toPeer: any SynchronizationPeerID) -> Bool

Transfers ownership of the given entity to the named network device.

**Required**

### Finding an entity

func entity(for: Self.Identifier) -> Entity?

Gets the entity with the given identifier.

**Required**

### Type Aliases

typealias Identifier

A type that represents a synchronization service identifier.

## Relationships

### Conforming Types

- MultipeerConnectivityService

## See Also

### Entity ownership synchronization

typealias Identifier

A type that represents a synchronization service identifier.

protocol SynchronizationPeerID

A type that represents a peer among a group of networked devices.

struct SynchronizationComponent

A component that synchronizes an entity between processes and networked applications.

enum OwnershipTransferMode

Modes of ownership transfer.

enum OwnershipTransferCompletionResult

The result of an ownership transfer request.

enum SynchronizationEvents

Events associated with network synchronization of scene information.

protocol HasSynchronization

An interface that enables an entity to be synchronized between processes and networked applications.

