

- GameplayKit
- GKNoise
-  remapValues(toTerracesWithPeaks:terracesInverted:) 

Instance Method

# remapValues(toTerracesWithPeaks:terracesInverted:)

Replaces values in the noise field by mapping them to a terrace-like curve that passes through the specified control points.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func remapValues(
    toTerracesWithPeaks peakInputValues: [NSNumber],
    terracesInverted inverted: Bool
)
```

## Parameters 

`peakInputValues`  

An array of noise values to use as the sharp points of the mapping curve.

`inverted`  

true for curves that start rising slowly and become more steep; false for curves that start rising quickly and become more shallow.

## Discussion

When you call this method, the GKNoise class first creates a curve between the points in the `peakInputValues` array. Each point in the array is a value that remains unchanged, and the `inverted` parameter determines the shape of the curve in between those points. Then, this method uses the curve to replace values in the noise field. The resulting effect can be useful for generating textures that resemble realistic terrain, replacing sloping hills with dramatic plateaus and ridges.

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

func remapValues(toCurveWithControlPoints: [NSNumber : NSNumber])

Replaces values in the noise field by mapping them to a curve that passes through the specified control points.

