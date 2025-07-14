

- PHASE
- PHASEBlendNodeDefinition
-  init(spatialMixerDefinition:identifier:) 

Initializer

# init(spatialMixerDefinition:identifier:)

Creates a named blend node for spatial audio output.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
convenience init(
    spatialMixerDefinition: PHASESpatialMixerDefinition,
    identifier: String
)
```

## Parameters 

`spatialMixerDefinition`  

An object that combines spatial audio layers.

`identifier`  

A unique name for the node.

## See Also

### Creating a Blend Node

init(blendMetaParameterDefinition: PHASENumberMetaParameterDefinition)

Creates a blend node with a maxiumum blend range value.

convenience init(blendMetaParameterDefinition: PHASENumberMetaParameterDefinition, identifier: String)

Creates a named blend node with a maxiumum blend range value.

init(spatialMixerDefinition: PHASESpatialMixerDefinition)

Creates a blend node for spatial audio output.

