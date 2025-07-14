

- RealityKit
- AnchoringComponent
-  AnchoringComponent.PhysicsSimulation 

Enumeration

# AnchoringComponent.PhysicsSimulation

Describes the physics simulation space of the entity and its descendants.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum PhysicsSimulation
```

## Overview

This allows developers to fine-tune which entities with an `AnchoringComponent` interact with each other physically, as opposed to not interacting at all.

## Topics

### Operators

static func == (AnchoringComponent.PhysicsSimulation, AnchoringComponent.PhysicsSimulation) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case isolated

Simulates the entity and its descendants in the entity’s own physics space.

case none

Opts out the entity and its descendants from having their own physics space.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

