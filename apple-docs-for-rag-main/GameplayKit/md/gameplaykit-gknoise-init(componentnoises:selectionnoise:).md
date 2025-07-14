

- GameplayKit
- GKNoise
-  init(componentNoises:selectionNoise:) 

Initializer

# init(componentNoises:selectionNoise:)

Creates a noise object by combining the specified noise objects, using another noise object to select which regions of the output correspond to which input noise.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
convenience init(
    componentNoises noises: [GKNoise],
    selectionNoise: GKNoise
)
```

## Parameters 

`noises`  

The array of noise objects to combine.

`selectionNoise`  

A noise object whose values determine which object from the `noises` array contributes to which region of the generated output.

## Return Value

A new noise object.

## Discussion

This method is equivalent to the init(componentNoises:selectionNoise:componentBoundaries:boundaryBlendDistances:) method, but automatically determines uniformly spaced boundaries based on the number of noise objects in the `noises` array, and using a blend distance of zero for each boundary. Together with these boundaries, the `selectionNoise` parameter determines which of the input noise objects appears in which region of generated noise.

For example, if the `noises` array contains two noise objects, the boundary value is zero: In regions where the `selectionNoise` field has negative values, the noise created by this method uses values from the first element of the `noises` array, and in regions where the `selectionNoise` field has positive values, the created noise uses values from the second element in the `noises` array.

## See Also

### Creating Noise by Combining Noise

convenience init(componentNoises: [GKNoise], selectionNoise: GKNoise, componentBoundaries: [NSNumber], boundaryBlendDistances: [NSNumber])

Creates a noise object by combining the specified noise objects, using another noise object and the specified boundaries to select which regions of the output correspond to which input noise.

