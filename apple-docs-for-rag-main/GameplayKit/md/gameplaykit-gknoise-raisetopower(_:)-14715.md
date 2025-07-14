

- GameplayKit
- GKNoise
-  raiseToPower(\_:) 

Instance Method

# raiseToPower(\_:)

Replaces all values in the noise field by raising each value to the specified power.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func raiseToPower(_ power: Double)
```

## Parameters 

`power`  

The exponent to raise each noise value to.

## Discussion

Noise values range from `-1.0` to `1.0`, so exponentiating always results in lower values than in the original noise, with a greater effect on low original values than on high values.

## See Also

### Applying Operations to Noise Values

func applyAbsoluteValue()

Replaces all negative values in the noise field with their positive absolute values.

func invert()

Replaces all values in the noise field with their opposite, reversing the range of noise values.

func clamp(lowerBound: Double, upperBound: Double)

Replaces values in the noise field outside the specified range with the values at the endpoints of that range.

func remapValues(toCurveWithControlPoints: [NSNumber : NSNumber])

Replaces values in the noise field by mapping them to a curve that passes through the specified control points.

func remapValues(toTerracesWithPeaks: [NSNumber], terracesInverted: Bool)

Replaces values in the noise field by mapping them to a terrace-like curve that passes through the specified control points.

