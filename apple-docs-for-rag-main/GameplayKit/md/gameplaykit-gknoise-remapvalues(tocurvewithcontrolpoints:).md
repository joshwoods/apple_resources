

- GameplayKit
- GKNoise
-  remapValues(toCurveWithControlPoints:) 

Instance Method

# remapValues(toCurveWithControlPoints:)

Replaces values in the noise field by mapping them to a curve that passes through the specified control points.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func remapValues(toCurveWithControlPoints controlPoints: [NSNumber : NSNumber])
```

## Parameters 

`controlPoints`  

A dictionary whose keys are input values in the existing noise, and whose values are the output values to replace the input values with.

## Discussion

When you call this method, the GKNoise class first interpolates the values specified in the `controlPoints` parameter to create a smooth curve. Then, this method uses the curve to replace values in the noise field. For example, passing the control points `[-1.0: -1.0, -0.5: 0.5, 0.5: -0.5, 1.0: 1.0]` defines an S-shaped curve that leaves the lowest and highest values in the noise field unchanged, but replaces moderately low values with moderately high values and vice versa.

## See Also

### Applying Operations to Noise Values

func applyAbsoluteValue()

Replaces all negative values in the noise field with their positive absolute values.

func invert()

Replaces all values in the noise field with their opposite, reversing the range of noise values.

func raiseToPower(Double)

Replaces all values in the noise field by raising each value to the specified power.

func clamp(lowerBound: Double, upperBound: Double)

Replaces values in the noise field outside the specified range with the values at the endpoints of that range.

func remapValues(toTerracesWithPeaks: [NSNumber], terracesInverted: Bool)

Replaces values in the noise field by mapping them to a terrace-like curve that passes through the specified control points.

