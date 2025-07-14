

- RealityKit
- SynchronizationComponent
-  SynchronizationComponent.OwnershipTransferMode 

Enumeration

# SynchronizationComponent.OwnershipTransferMode

Modes of ownership transfer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
enum OwnershipTransferMode
```

## Topics

### Ownership transfer modes

case autoAccept

Grant ownership requests automatically.

case manual

Require explicit ownership request confirmation.

### Comparing ownership transfer modes

static func == (SynchronizationComponent.OwnershipTransferMode, SynchronizationComponent.OwnershipTransferMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Entity ownership synchronization

protocol SynchronizationService

An interface that enables entity synchronization among a group of local peers.

typealias Identifier

A type that represents a synchronization service identifier.

protocol SynchronizationPeerID

A type that represents a peer among a group of networked devices.

struct SynchronizationComponent

A component that synchronizes an entity between processes and networked applications.

enum OwnershipTransferCompletionResult

The result of an ownership transfer request.

enum SynchronizationEvents

Events associated with network synchronization of scene information.

protocol HasSynchronization

An interface that enables an entity to be synchronized between processes and networked applications.

