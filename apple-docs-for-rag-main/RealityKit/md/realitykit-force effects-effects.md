

- RealityKit
-  Force effects 

API Collection

# Force effects

Control the movement of virtual objects with forces.

## Overview

Create various types of force effects, such as vortex, drag, and turbulence. Add a force effect to a scene by creating a structure that adopts ForceEffectProtocol, and attaching it to an entity with a ForceEffectComponent.

## Topics

### Force effect components

struct ForceEffectComponent

A component that defines the forces that affect an entity, including custom forces that you define.

struct ForceEffect

Defines a force effect’s system, and type specific properties.

### Built-in force effect types

struct ConstantForceEffect

A force effect that exerts a constant force in a direction relative to the effect’s transform.

struct ConstantRadialForceEffect

A force effect that pulls objects toward its center with a constant strength.

struct DragForceEffect

A force effect that slows bodies within its area of effect with a force proportional to the body’s velocity.

struct RadialForceEffect

A force effect that pulls objects toward its center with a spring-like (distance dependent) force.

struct TurbulenceForceEffect

A force effect that applies random forces with magnitudes proportional to each body’s velocity.

struct VortexForceEffect

A force effect whose forces circulate around an axis centered at the origin of the effect.

### Force effect constraints

enum ForceEffectBounds

The boundary options for a force effect.

struct SpatialForceFalloff

A type that modulates the force strength based on the distance of rigid bodies.

struct TimedForceFalloff

A type that modulates the force strength based on how long the force effect has run.

### Custom forces

protocol ForceEffectProtocol

A protocol that defines a custom force effect.

enum ForceMode

The options that control how physics system applies the forces.

struct ForceEffectParameters

The force effect input data to the effect’s update handler or closure.

protocol ForceEffectBase

The base protocol for the wrapping force effect structure containing common parameters for all force-effects.

## See Also

### Physics simulation

Collision detection

Determine when entities collide with each other or the environment.

Simulations and motion

Simulate physical interactions between entities or systems.

Physics joints and pins

Simulate joint physics that connect virtual objects.

