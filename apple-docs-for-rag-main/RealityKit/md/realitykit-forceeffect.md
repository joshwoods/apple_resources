

- RealityKit
-  ForceEffect 

Structure

# ForceEffect

Defines a force effect’s system, and type specific properties.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ForceEffect where ForceEffectType : ForceEffectProtocol
```

## Overview

This struct wraps your custom force effect that conforms to ForceEffectProtocol and provides properties that are common to all force effects.

## Topics

### Initializers

init(effect: ForceEffectType, strengthScale: Double, spatialFalloff: SpatialForceFalloff?, timedFalloff: TimedForceFalloff?, position: SIMD3&lt;Float>, orientation: simd_quatf, mask: CollisionGroup)

Creates a ForceEffect struct.

### Instance Properties

var effect: ForceEffectType

Parameters that can vary for different types.

var mask: CollisionGroup

Controls which collision groups will be affected by this force effect.

var orientation: simd_quatf

Rotation of the force effect relative to the effect’s transform component.

var position: SIMD3&lt;Float>

Position of the force effect relative to the effect’s transform component.

var spatialFalloff: SpatialForceFalloff?

Optional strength falloff based on the spatial bounds of the effect.

var strengthScale: Float

A multiplier that scales the strength of the effect.

var timedFalloff: TimedForceFalloff?

Optional strength falloff based on the duration of the effect.

## Relationships

### Conforms To

- ForceEffectBase

## See Also

### Force effect components

struct ForceEffectComponent

A component that defines the forces that affect an entity, including custom forces that you define.

