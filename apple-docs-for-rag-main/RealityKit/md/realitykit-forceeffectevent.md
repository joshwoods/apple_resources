

- RealityKit
-  ForceEffectEvent 

Structure

# ForceEffectEvent

A struct that defines the arguments to the custom force effect update closure.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ForceEffectEvent where ForceEffectType : ForceEffectProtocol
```

## Overview

If you register your custom force effect using a closure, you can access the force effect’s property and ForceEffectParameters from this struct.

## Topics

### Instance Properties

var effect: ForceEffectType

The force effect to update.

var parameters: ForceEffectParameters

Physics body parameters.

## See Also

### Updating effects

func update(parameters: inout ForceEffectParameters)

Defines how the custom force effect computes forces at each physics simulation step.

**Required** Default implementation provided.

static func register(((inout ForceEffectEvent&lt;Self>) -> Void)?)

Registers the custom effect.

struct PhysicsBodyParameterTypes

Defines which rigid body inputs are required by a force effect’s update handler.

struct ForceEffectParameters

The force effect input data to the effect’s update handler or closure.

struct UnsafeForceEffectBuffer

Provides access to physics body parameters from the effect’s update function or event handler.

