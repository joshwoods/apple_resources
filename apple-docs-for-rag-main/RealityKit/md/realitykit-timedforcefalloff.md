

- RealityKit
-  TimedForceFalloff 

Structure

# TimedForceFalloff

A type that modulates the force strength based on how long the force effect has run.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct TimedForceFalloff
```

## Overview

Forces have the largest strength when the force effect starts to play and gradually decay to zero when approaching the given duration. The effect also stops playing when reaching the duration.

Similar to SpatialForceFalloff, rate controls how fast the force strength decays. You can set the rate to zero to have a force effect with no temporal falloff.

```
let noTimedFalloff = TimedFalloff(duration: 1, rate: 0)
```

## Topics

### Initializers

init(duration: TimeInterval, rate: Double)

Creates a timed force falloff.

### Instance Properties

var duration: TimeInterval

The lifetime of the effect in seconds.

var rate: Double

The temporal falloff / attenuation rate.

## See Also

### Force effect constraints

enum ForceEffectBounds

The boundary options for a force effect.

struct SpatialForceFalloff

A type that modulates the force strength based on the distance of rigid bodies.

