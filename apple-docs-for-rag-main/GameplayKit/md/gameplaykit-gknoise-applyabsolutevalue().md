

- GameplayKit
- GKNoise
-  applyAbsoluteValue() 

Instance Method

# applyAbsoluteValue()

Replaces all negative values in the noise field with their positive absolute values.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func applyAbsoluteValue()
```

## Discussion

For example, a value of `-0.75` becomes `0.75`, but positive values such as `0.5` remain unchanged.

## See Also

### Applying Operations to Noise Values

func invert()

Replaces all values in the noise field with their opposite, reversing the range of noise values.

func raiseToPower(Double)

Replaces all values in the noise field by raising each value to the specified power.

func clamp(lowerBound: Double, upperBound: Double)

Replaces values in the noise field outside the specified range with the values at the endpoints of that range.

func remapValues(toCurveWithControlPoints: [NSNumber : NSNumber])

Replaces values in the noise field by mapping them to a curve that passes through the specified control points.

func remapValues(toTerracesWithPeaks: [NSNumber], terracesInverted: Bool)

Replaces values in the noise field by mapping them to a terrace-like curve that passes through the specified control points.

