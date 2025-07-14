

- RealityKit
-  ForceEffectBase 

Protocol

# ForceEffectBase

The base protocol for the wrapping force effect structure containing common parameters for all force-effects.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
protocol ForceEffectBase
```

## Overview

Don’t implement this protocol yourself. Create force effects by calling methods on ForceEffect.

## Topics

### Associated Types

associatedtype ForceEffectType : ForceEffectProtocol

A type that represents the kind of force effect.

**Required**

### Instance Properties

var effect: Self.ForceEffectType

Custom force effect parameters.

**Required**

var mask: CollisionGroup

Controls which collision groups will be affected by this force effect.

**Required**

var orientation: simd_quatf

Rotation of the force effect relative to the effect’s transform component.

**Required**

var position: SIMD3&lt;Float>

Position of the force effect relative to the effect’s transform component.

**Required**

var spatialFalloff: SpatialForceFalloff?

Optional strength falloff based on the spatial bounds of the effect.

**Required**

var strengthScale: Float

A multiplier that scales the strength of the effect.

**Required**

var timedFalloff: TimedForceFalloff?

Optional strength falloff based on the duration of the effect.

**Required**

## Relationships

### Conforming Types

- ForceEffect

## See Also

### Custom forces

protocol ForceEffectProtocol

A protocol that defines a custom force effect.

enum ForceMode

The options that control how physics system applies the forces.

struct ForceEffectParameters

The force effect input data to the effect’s update handler or closure.

