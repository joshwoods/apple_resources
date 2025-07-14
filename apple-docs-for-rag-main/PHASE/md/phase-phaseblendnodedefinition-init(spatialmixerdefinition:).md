

- PHASE
- PHASEBlendNodeDefinition
-  init(spatialMixerDefinition:) 

Initializer

# init(spatialMixerDefinition:)

Creates a blend node for spatial audio output.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
init(spatialMixerDefinition: PHASESpatialMixerDefinition)
```

## Parameters 

`spatialMixerDefinition`  

An object that combines spatial audio layers.

## See Also

### Creating a Blend Node

init(blendMetaParameterDefinition: PHASENumberMetaParameterDefinition)

Creates a blend node with a maxiumum blend range value.

convenience init(blendMetaParameterDefinition: PHASENumberMetaParameterDefinition, identifier: String)

Creates a named blend node with a maxiumum blend range value.

convenience init(spatialMixerDefinition: PHASESpatialMixerDefinition, identifier: String)

Creates a named blend node for spatial audio output.

