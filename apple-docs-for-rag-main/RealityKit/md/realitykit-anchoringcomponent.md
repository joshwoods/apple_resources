

- RealityKit
-  AnchoringComponent 

Structure

# AnchoringComponent

A component that anchors virtual content to a real world target.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS

``` source
struct AnchoringComponent
```

## Overview

This component is essential for getting AR features into RealityKit. Use `AnchoringComponent` to anchor virtual content to a real world target by attaching the component to any Entity in your RealityKit scene.

To create an `AnchoringComponent`, you need to specify a AnchoringComponent.Target. You can also specify the AnchoringComponent.TrackingMode and the AnchoringComponent.PhysicsSimulation to control how the entity tracks the anchor and how the physics simulates with the entity.

For example, here’s how to create an entity that targets the left hand’s wrist with predicted tracking mode:

```
let target = AnchoringComponent.Target.hand(.left, location: .wrist)
let anchoringComponent = AnchoringComponent(target, trackingMode: .predicted)
let entity = Entity()
entity.components.set(anchoringComponent)
```

The entity with `AnchoringComponent` is inactive when created. RealityKit anchors and activates the entity when it finds an anchor that meets the target requirements. You can check the entity’s anchored status using isAnchored, or you can subscribe to SceneEvents.AnchoredStateChanged events to receive scene events.

Similarly, RealityKit unanchors the entity if the target disappears or no longer meets the target requirements.

For more information about anchors, see ARKit.

## Topics

### Creating the anchor component

init(AnchoringComponent.Target)

Creates an anchoring component for a given target.

init(AnchoringComponent.Target, trackingMode: AnchoringComponent.TrackingMode)

init(AnchoringComponent.Target, trackingMode: AnchoringComponent.TrackingMode, physicsSimulation: AnchoringComponent.PhysicsSimulation)

Creates an anchoring component for a given target, tracking mode and physics simulation.

init(ARAnchor)

Creates an anchoring component with the given AR anchor.

### Setting a target

let target: AnchoringComponent.Target

The real world anchor target to attach the entity to.

### Setting a tracking mode

var trackingMode: AnchoringComponent.TrackingMode

Defines how the `Entity` tracks its target anchor.

### Setting a physics simulation space

var physicsSimulation: AnchoringComponent.PhysicsSimulation

Specifies the physics simulation spece that the entity and its descendants are in.

### Registering a component type

static func registerComponent()

Registers a new component type.

### Comparing anchoring components

static func == (AnchoringComponent, AnchoringComponent) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Structures

struct ImageAnchoringSource

Defines the source of object anchoring target based on how it is created.

struct ObjectAnchoringSource

Defines the source of object anchoring target based on how it is created.

struct TrackingMode

Decides how the `Entity` tracks its target anchor.

### Enumerations

enum PhysicsSimulation

Describes the physics simulation space of the entity and its descendants.

enum Target

Defines the kinds of real world objects to which an anchor entity can be tethered.

### Default Implementations

Component Implementations

Equatable Implementations

## Relationships

### Conforms To

- Component
- Equatable

## See Also

### Anchoring component

enum Target

Defines the kinds of real world objects to which an anchor entity can be tethered.

struct TrackingMode

Decides how the `Entity` tracks its target anchor.

class AnchorEntity

An anchor that tethers entities to a scene.

protocol HasAnchoring

An interface that enables anchoring of virtual content to a real-world object in an AR scene.

