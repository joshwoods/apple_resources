

- PHASE
- PHASEDucker
-  attackTime 

Instance Property

# attackTime

The amount of time for sound reduction to reach maximum strength.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var attackTime: Double { get }
```

## See Also

### Configuring Volume Reduction

var gain: Double

The amount of volume reduction.

var identifier: String

A unique value for the ducker.

var isActive: Bool

A Boolean value that determines whether the ducker reduces sound.

var attackCurve: PHASECurveType

A mathematical curve that shapes transition progress as sound reduction begins.

var releaseTime: Double

The amount of time to transition from maximum sound reduction to no reduction.

var releaseCurve: PHASECurveType

A mathematical curve that shapes transition progress as sound reduction ends.

