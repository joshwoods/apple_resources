

- RealityKit
-  HasHierarchy 

Protocol

# HasHierarchy

An interface that provides access to a parent entity and child entities.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
protocol HasHierarchy : Entity
```

## Mentioned in 

Loading entities from a file

## Overview

All entities automatically adopt this protocol because the Entity base class does. This adoption gives all entities a collection of methods for managing the hierarchy.

## Topics

### Managing the parent

var parent: Entity?

The parent entity.

func setParent(Entity?, preservingWorldTransform: Bool)

Attaches the entity as a child to the specified entity.

func removeFromParent(preservingWorldTransform: Bool)

Removes the entity from its current parent or from the scene if it is a root entity.

### Managing children

var children: Entity.ChildCollection

The child entities that the entity manages.

func addChild(Entity, preservingWorldTransform: Bool)

Adds the given entity to the collection of child entities.

func removeChild(Entity, preservingWorldTransform: Bool)

Removes the given child from the entity.

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

### Relating entities

var parent: Entity?

The parent entity.

func setParent(Entity?, preservingWorldTransform: Bool)

Attaches the entity as a child to the specified entity.

func removeFromParent(preservingWorldTransform: Bool)

Removes the entity from its current parent or from the scene if it is a root entity.

var children: Entity.ChildCollection

The child entities that the entity manages.

func addChild(Entity, preservingWorldTransform: Bool)

Adds the given entity to the collection of child entities.

func removeChild(Entity, preservingWorldTransform: Bool)

Removes the given child from the entity.

struct ChildCollection

A collection of child entities.

