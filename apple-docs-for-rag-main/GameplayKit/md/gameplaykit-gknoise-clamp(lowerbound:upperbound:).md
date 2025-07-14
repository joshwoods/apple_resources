

- GameplayKit
- GKNoise
-  clamp(lowerBound:upperBound:) 

Instance Method

# clamp(lowerBound:upperBound:)

Replaces values in the noise field outside the specified range with the values at the endpoints of that range.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func clamp(
    lowerBound: Double,
    upperBound: Double
)
```

## Parameters 

`lowerBound`  

The minimum value to keep in processed noise.

`upperBound`  

The maximum value to keep in processed noise.

## Discussion

For example, if you specify lower and upper bounds of `-0.5` and `0.5`, this operation replaces values less than `-0.5` with `-0.5` and values greater than `0.5` with `0.5`.

## See Also

### Applying Operations to Noise Values

func applyAbsoluteValue()

Replaces all negative values in the noise field with their positive absolute values.

func invert()

Replaces all values in the noise field with their opposite, reversing the range of noise values.

func raiseToPower(Double)

Replaces all values in the noise field by raising each value to the specified power.

func remapValues(toCurveWithControlPoints: [NSNumber : NSNumber])

Replaces values in the noise field by mapping them to a curve that passes through the specified control points.

func remapValues(toTerracesWithPeaks: [NSNumber], terracesInverted: Bool)

Replaces values in the noise field by mapping them to a terrace-like curve that passes through the specified control points.

