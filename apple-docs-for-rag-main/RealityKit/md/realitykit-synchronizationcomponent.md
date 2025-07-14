

- RealityKit
-  SynchronizationComponent 

Structure

# SynchronizationComponent

A component that synchronizes an entity between processes and networked applications.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct SynchronizationComponent
```

## Overview

An entity acquires a SynchronizationComponent instance by adopting the HasSynchronization protocol. All entities have this component because the Entity base class adopts the protocol.

## Topics

### Creating a synchronization component

init()

Creates a synchronization component.

### Identifying a synchronization component

var identifier: UInt64

A unique identifier of an entity within a network session.

### Managing ownership

var isOwner: Bool

A Boolean that indicates whether the calling process owns the entity.

var ownershipTransferMode: SynchronizationComponent.OwnershipTransferMode

The entity’s transfer ownership mode.

### Registering a component type

static func registerComponent()

Registers a new component type.

### Comparing synchronization components

static func == (SynchronizationComponent, SynchronizationComponent) -> Bool

Indicates whether two synchronization components are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Enumerations

enum OwnershipTransferCompletionResult

The result of an ownership transfer request.

enum OwnershipTransferMode

Modes of ownership transfer.

### Default Implementations

Component Implementations

Equatable Implementations

## Relationships

### Conforms To

- Component
- Equatable

## See Also

### Entity ownership synchronization

protocol SynchronizationService

An interface that enables entity synchronization among a group of local peers.

typealias Identifier

A type that represents a synchronization service identifier.

protocol SynchronizationPeerID

A type that represents a peer among a group of networked devices.

enum OwnershipTransferMode

Modes of ownership transfer.

enum OwnershipTransferCompletionResult

The result of an ownership transfer request.

enum SynchronizationEvents

Events associated with network synchronization of scene information.

protocol HasSynchronization

An interface that enables an entity to be synchronized between processes and networked applications.

