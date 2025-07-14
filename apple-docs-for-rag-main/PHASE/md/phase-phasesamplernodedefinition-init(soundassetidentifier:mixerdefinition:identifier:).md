

- PHASE
- PHASESamplerNodeDefinition
-  init(soundAssetIdentifier:mixerDefinition:identifier:) 

Initializer

# init(soundAssetIdentifier:mixerDefinition:identifier:)

Creates a named sampler node with the given sound asset and mixer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
convenience init(
    soundAssetIdentifier: String,
    mixerDefinition: PHASEMixerDefinition,
    identifier: String
)
```

## Parameters 

`soundAssetIdentifier`  

A name that refers to the audio data that the node plays. See assetIdentifier.

`mixerDefinition`  

An object that combines audio layers.

`identifier`  

A unique name for the sample node.

## See Also

### Creating a Sampler Node

init(soundAssetIdentifier: String, mixerDefinition: PHASEMixerDefinition)

Creates a sampler node with the given sound asset and mixer.

