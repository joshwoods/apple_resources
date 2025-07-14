

- RealityKit
- ForceEffectProtocol
-  register(\_:) 

Type Method

# register(\_:)

Registers the custom effect.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
static func register(_ updateHandler: (@MainActor (inout ForceEffectEvent) -> Void)? = nil)
```

## Parameters 

`updateHandler`  

A closure that computes custom forces for rigid bodies.

## Discussion

If a handler is specified, the physics system calls the handler and ignores the update function.

## See Also

### Updating effects

func update(parameters: inout ForceEffectParameters)

Defines how the custom force effect computes forces at each physics simulation step.

**Required** Default implementation provided.

struct PhysicsBodyParameterTypes

Defines which rigid body inputs are required by a force effect’s update handler.

struct ForceEffectParameters

The force effect input data to the effect’s update handler or closure.

struct ForceEffectEvent

A struct that defines the arguments to the custom force effect update closure.

struct UnsafeForceEffectBuffer

Provides access to physics body parameters from the effect’s update function or event handler.

