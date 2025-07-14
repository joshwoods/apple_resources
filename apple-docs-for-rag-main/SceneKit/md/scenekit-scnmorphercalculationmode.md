

- SceneKit
-  SCNMorpherCalculationMode 

Enumeration

# SCNMorpherCalculationMode

The interpolation formulas for blending between target geometries.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum SCNMorpherCalculationMode
```

## Overview

A morpher computes its current surface by summing weighted geometry elements from the base geometry and all target geometries. The position of a vertex on the surface is produced by adding the position vector of a point on the base geometry to the position vectors of the corresponding points on all target geometries. The morpher’s calculationMode property selects the formula used to calculate this sum.

If the mode is SCNMorpherCalculationMode.normalized, the position from the base geometry is weighted by one minus the sum of all target weights, as in the following formula:

```
Position = (1 - weight0 - weight1 - ...) * Base + weight0 * Target0 + weight1 * Target1 + ...
```

If the mode is SCNMorpherCalculationMode.additive, the position from the base geometry is not weighted, and SceneKit uses the following formula instead:

```
Position = Base + weight0 * Target0 + weight1 * Target1 + ...
```

## Topics

### Constants

case normalized

Target weights must be in the range between `0.0` and `1.0`, and the contribution of the base geometry to the morphed surface is related to the sum of target weights. This is the default mode.

case additive

Target weights may take on any value, and weighted contributions for each target are added to the base geometry,

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

