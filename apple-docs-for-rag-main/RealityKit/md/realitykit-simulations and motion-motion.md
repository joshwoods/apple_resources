

- RealityKit
-  Simulations and motion 

API Collection

# Simulations and motion

Simulate physical interactions between entities or systems.

## Overview

RealityKit simulates physical interactions between virtual objects in your scene, as well as between virtual objects and detected surfaces in the real world, such as floors, walls, or tabletops. On devices with a LiDAR Scanner, RealityKit can even simulate interactions between virtual objects and scanned real-world geometry.

## Topics

### Simulation setup

Designing scene hierarchies for efficient physics simulation

Configure your RealityKit scenes to avoid performance bottlenecks.

Handling different-sized objects in physics simulations

Set up a scene hierarchy for accurate physics simulations.

struct PhysicsSimulationComponent

A component that controls localized physics simulations.

### Simulation-related notifications

enum PhysicsSimulationEvents

Types of events that fire during physics simulations

### Physical properties

struct PhysicsBodyComponent

A component that defines an entity’s behavior in physics body simulations.

class PhysicsMaterialResource

Material properties, like friction, of a physically simulated object.

enum PhysicsBodyMode

The ways that a physics body can move in response to physical forces.

struct PhysicsMassProperties

Mass properties of a physics body.

### Physics motion

struct PhysicsMotionComponent

A component that controls the motion of the body in physics simulations.

struct ImpulseAction

An action that applies an impulse to the physics body at its center of mass when played as an animation.

### Particle simulation

Simulating particles in your visionOS app

Add a range of visual effects to a RealityKit view by attaching a particle emitter component to an entity.

struct ParticleEmitterComponent

A component that emits particles.

struct ParticleEmitter

struct Presets

Initial configurations that can be set when starting a new simulation.

### Entity compliance

protocol HasPhysicsBody

An interface that enables physics simulations based on the rules of Newtonian mechanics.

protocol HasPhysicsMotion

An interface that provides velocity properties for physics simulations.

protocol HasPhysics

An interface that combines the physics body and physics motion interfaces.

## See Also

### Physics simulation

Collision detection

Determine when entities collide with each other or the environment.

Force effects

Control the movement of virtual objects with forces.

Physics joints and pins

Simulate joint physics that connect virtual objects.

