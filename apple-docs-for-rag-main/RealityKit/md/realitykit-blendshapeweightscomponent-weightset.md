

- RealityKit
- BlendShapeWeightsComponent
-  weightSet 

Instance Property

# weightSet

The runtime named blend shapes weights.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var weightSet: BlendShapeWeightsSet { get set }
```

## Discussion

Initialize the `weightSet` variable using the init() function.

The `weightSet` variable has the following limitations as to how it can be set:

- If `weightSet` is assigned to a new BlendShapeWeightsSet, then the new set have the same number of weights and weight names as the current variable. Additionally, make sure the weight names exactly match the current set’s weight names.

- Weight name changes are ignored.

- Setting an incorrect number of weight values are ignored.

- Blend shape name changes are ignored.

