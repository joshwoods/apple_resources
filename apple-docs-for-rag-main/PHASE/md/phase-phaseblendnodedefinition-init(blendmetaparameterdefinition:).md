

- PHASE
- PHASEBlendNodeDefinition
-  init(blendMetaParameterDefinition:) 

Initializer

# init(blendMetaParameterDefinition:)

Creates a blend node with a maxiumum blend range value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
init(blendMetaParameterDefinition: PHASENumberMetaParameterDefinition)
```

## Parameters 

`blendMetaParameterDefinition`  

A maximum value for the blend range. The sound event’s blend meta parameter across a range from `0` to this value produces an active cross-fade along the child nodes.

## See Also

### Creating a Blend Node

convenience init(blendMetaParameterDefinition: PHASENumberMetaParameterDefinition, identifier: String)

Creates a named blend node with a maxiumum blend range value.

init(spatialMixerDefinition: PHASESpatialMixerDefinition)

Creates a blend node for spatial audio output.

convenience init(spatialMixerDefinition: PHASESpatialMixerDefinition, identifier: String)

Creates a named blend node for spatial audio output.

