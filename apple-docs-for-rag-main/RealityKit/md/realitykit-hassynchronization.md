

- RealityKit
-  HasSynchronization 

Protocol

# HasSynchronization

An interface that enables an entity to be synchronized between processes and networked applications.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
protocol HasSynchronization : Entity
```

## Overview

All entities automatically adopt this protocol because the Entity base class does. This adoption gives all entities a SynchronizationComponent instance, and a collection of methods for manipulating the component, that you use to manage ownership of the entity.

## Topics

### Accessing the component

var synchronization: SynchronizationComponent?

The entity’s synchronization component.

### Managing ownership

var isOwner: Bool

A Boolean that indicates whether the calling process owns the entity.

func requestOwnership(timeout: TimeInterval, (SynchronizationComponent.OwnershipTransferCompletionResult) -> Void)

Requests ownership of the entity.

### Making local changes

func withUnsynchronized(() -> Void)

Calls the given closure in a way such that component changes that the closure makes don’t trigger synchronization.

## Relationships

### Inherits From

- Entity

### Conforming Types

- AnchorEntity
- BodyTrackedEntity
- DirectionalLight
- Entity
- ModelEntity
- PerspectiveCamera
- PointLight
- SpotLight
- TriggerVolume
- ViewAttachmentEntity

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

enum OwnershipTransferMode

Modes of ownership transfer.

enum OwnershipTransferCompletionResult

The result of an ownership transfer request.

enum SynchronizationEvents

Events associated with network synchronization of scene information.

