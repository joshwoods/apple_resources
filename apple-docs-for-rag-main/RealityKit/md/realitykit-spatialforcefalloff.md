

- RealityKit
-  SpatialForceFalloff 

Structure

# SpatialForceFalloff

A type that modulates the force strength based on the distance of rigid bodies.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct SpatialForceFalloff
```

## Overview

Forces applied to rigid bodies near the effect’s origin have the largest strength and gradually decay to zero when approaching the boundary of ForceEffectBounds.

rate controls how fast the force strength decays. Under the hood the rate is an exponent of the normalized distance over the spatial bounds. For example when the rate is 0, the falloff coefficient (i.e. distance raised to the power of 0) is constantly 1, and that implies no decay or falloff the force strength.

```
let noFalloff = SpatialForceFalloff(bounds: .sphere(radius: 10), rate: 0)
```

As another example, you can set rate to `1` to decay the force strength linearly.

```
let linearFalloff = SpatialForceFalloff(bounds: .sphere(radius: 10), rate: 1)
```

## Topics

### Initializers

init(bounds: ForceEffectBounds, rate: Double, distanceOffset: Double)

Creates a spatial force falloff.

### Instance Properties

var bounds: ForceEffectBounds

The spatial bounds that define the area over which the force effect’s strength decreases.

var distanceOffset: Double

A distance from the origin where the falloff begins.

var rate: Double

The spatial falloff / attenuation rate.

## See Also

### Force effect constraints

enum ForceEffectBounds

The boundary options for a force effect.

struct TimedForceFalloff

A type that modulates the force strength based on how long the force effect has run.

