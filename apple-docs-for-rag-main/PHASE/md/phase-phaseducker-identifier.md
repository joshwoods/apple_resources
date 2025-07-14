

- PHASE
- PHASEDucker
-  identifier 

Instance Property

# identifier

A unique value for the ducker.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var identifier: String { get }
```

## See Also

### Configuring Volume Reduction

var gain: Double

The amount of volume reduction.

var isActive: Bool

A Boolean value that determines whether the ducker reduces sound.

var attackTime: Double

The amount of time for sound reduction to reach maximum strength.

var attackCurve: PHASECurveType

A mathematical curve that shapes transition progress as sound reduction begins.

var releaseTime: Double

The amount of time to transition from maximum sound reduction to no reduction.

var releaseCurve: PHASECurveType

A mathematical curve that shapes transition progress as sound reduction ends.

