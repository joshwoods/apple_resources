

- RealityKit
-  ModelEntity 

Class

# ModelEntity

A representation of a physical object that RealityKit renders and optionally simulates.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
class ModelEntity
```

## Mentioned in 

Adding procedural assets to a scene

Reducing CPU Utilization in Your RealityKit App

Loading entities from a file

## Overview

Use one or more model entities to place physical objects in a scene. In addition to the components they inherit from the Entity class, model entities have geometry, described by their ModelComponent. Model entities acquire the model component by conforming to the HasModel protocol. You specify meshes and materials to control how a model entity appears.

Models respond to physics simulations because they conform to the HasPhysics protocol. You give them mass and other physical properties with a PhysicsBodyComponent instance, and then apply forces or impulses. The simulator uses a PhysicsMotionComponent to manage the linear and angular velocity of the object. Alternatively, you can selectively circumvent the simulation to control position and velocity yourself. Do this for a given model by setting its physics body mode to PhysicsBodyMode.kinematic.

Models can also collide with one another, and with other entities that conform to the HasCollision protocol. The CollisionComponent provides parameters that let you manage which models collide with each other. It also lets you control the collision shape, which for performance reasons, is typically simpler than the visual geometry.

## Topics

### Creating a model

init()

Creates a model entity.

init(mesh: MeshResource, materials: [any Material])

Creates a model entity with a particular mesh and set of materials.

init(mesh: MeshResource, materials: [any Material], collisionShape: ShapeResource, mass: Float)

Creates a model entity with a particular mesh, set of materials, collision shape, and mass.

init(mesh: MeshResource, materials: [any Material], collisionShapes: [ShapeResource], mass: Float)

Creates a model entity with a particular mesh, set of materials, a composite collision shape, and mass.

### Configuring the model

var model: ModelComponent?

The model component for the entity.

var jointNames: [String]

The names of all the joints in the model entity.

var jointTransforms: [Transform]

The relative joint transforms of the model entity.

### Detecting collisions

var collision: CollisionComponent?

The collision component that gives the entity the ability to participate in collision simulations.

### Simulating forces, impulses, and motion

var physicsBody: PhysicsBodyComponent?

A component that is used for physics simulations of the model entity in accordance with the laws of Newtonian mechanics.

var physicsMotion: PhysicsMotionComponent?

The physics motion component used by physics simulations of the model entity.

func addForce(SIMD3&lt;Float>, relativeTo: Entity?)

Applies a force to the physics body at its center of mass.

func addForce(SIMD3&lt;Float>, at: SIMD3&lt;Float>, relativeTo: Entity?)

Applies a force to the physics body at the specified position.

func addTorque(SIMD3&lt;Float>, relativeTo: Entity?)

Applies a torque to the physics body at its center of mass.

func clearForcesAndTorques()

Clears all forces previously added to the physics body.

func applyLinearImpulse(SIMD3&lt;Float>, relativeTo: Entity?)

Applies an impulse to the physics body at its center of mass.

func applyAngularImpulse(SIMD3&lt;Float>, relativeTo: Entity?)

Applies an angular (torque) impulse to the physics body at its center of mass.

func applyImpulse(SIMD3&lt;Float>, at: SIMD3&lt;Float>, relativeTo: Entity?)

Applies an impulse to the physics body at the specified position.

func resetPhysicsTransform(recursive: Bool)

Resets the position, orientation, and velocities of the simulated physics body.

func resetPhysicsTransform(Transform, recursive: Bool)

Resets the position and velocities of the simulated physics body.

Deprecated

### Default Implementations

HasCollision Implementations

HasModel Implementations

HasPhysicsBody Implementations

HasPhysicsMotion Implementations

## Relationships

### Inherits From

- Entity

### Conforms To

- CustomDebugStringConvertible
- Equatable
- EventSource
- HasCollision
- HasHierarchy
- HasModel
- HasPhysics
- HasPhysicsBody
- HasPhysicsMotion
- HasSynchronization
- HasTransform
- Hashable
- Identifiable
- RealityCoordinateSpace
- Sendable

## See Also

### Model display

struct ModelComponent

A component that contains a mesh and materials for the visual appearance of an entity.

class MeshResource

A high-level representation of a collection of vertices and edges that define a shape.

