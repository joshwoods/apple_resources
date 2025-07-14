

- PHASE
- PHASEBlendNodeDefinition
-  init(blendMetaParameterDefinition:identifier:) 

Initializer

# init(blendMetaParameterDefinition:identifier:)

Creates a named blend node with a maxiumum blend range value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
convenience init(
    blendMetaParameterDefinition: PHASENumberMetaParameterDefinition,
    identifier: String
)
```

## Parameters 

`blendMetaParameterDefinition`  

A maximum value for the blend range. The sound event’s blend meta parameter across a range from `0` to this value produces an active cross-fade along the child nodes.

`identifier`  

A unique name for the blend node.

## See Also

### Creating a Blend Node

init(blendMetaParameterDefinition: PHASENumberMetaParameterDefinition)

Creates a blend node with a maxiumum blend range value.

init(spatialMixerDefinition: PHASESpatialMixerDefinition)

Creates a blend node for spatial audio output.

convenience init(spatialMixerDefinition: PHASESpatialMixerDefinition, identifier: String)

Creates a named blend node for spatial audio output.

