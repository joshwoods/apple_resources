

- RealityKit
- BlendShapeWeightsMapping
-  init(blendShapeName:weightNames:) 

Initializer

# init(blendShapeName:weightNames:)

Creates a mapping that applies the weight names to mesh parts in a model component.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    blendShapeName: String,
    weightNames: [String]
)
```

## Parameters 

`blendShapeName`  

The user-defined name of the blend shape.

`weightNames`  

The names of the weights that are managed by this mapping.

## Discussion

This creates a mapping that applies the weight names to every mesh part in the ModelComponent associated with the BlendShapeWeightsComponent’s entity.

Make sure the weight names match the weight names in the mesh resource data. RealityKit will ignore weight names that do not match.

