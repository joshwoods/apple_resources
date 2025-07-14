

- RealityKit
- BlendShapeWeightsData
-  init(id:weights:) 

Initializer

# init(id:weights:)

Creates an instance of the named weights for a single blend shape.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    id: BlendShapeWeightsData.ID,
    weights: [(String, BlendShapeWeights.Element)]
)
```

## Parameters 

`id`  

The unique name of the blend shape.

`weights`  

An array of name value pairs for the weights in predefined order.

