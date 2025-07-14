

- RealityKit
- ForceEffectProtocol
-  update(parameters:) 

Instance Method

# update(parameters:)

Defines how the custom force effect computes forces at each physics simulation step.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
func update(parameters: inout ForceEffectParameters)
```

**Required** Default implementation provided.

## Parameters 

`parameters`  

On input, the rigid body parameters declared in parameterTypes. On output, the computed forces and torques.

## Default Implementations

### ForceEffectProtocol Implementations

func update(parameters: inout ForceEffectParameters)

Outputs zero forces and torques by default.

## See Also

### Updating effects

static func register(((inout ForceEffectEvent&lt;Self>) -> Void)?)

Registers the custom effect.

struct PhysicsBodyParameterTypes

Defines which rigid body inputs are required by a force effect’s update handler.

struct ForceEffectParameters

The force effect input data to the effect’s update handler or closure.

struct ForceEffectEvent

A struct that defines the arguments to the custom force effect update closure.

struct UnsafeForceEffectBuffer

Provides access to physics body parameters from the effect’s update function or event handler.

