

- PHASE
- PHASESamplerNodeDefinition
-  init(soundAssetIdentifier:mixerDefinition:) 

Initializer

# init(soundAssetIdentifier:mixerDefinition:)

Creates a sampler node with the given sound asset and mixer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
init(
    soundAssetIdentifier: String,
    mixerDefinition: PHASEMixerDefinition
)
```

## Parameters 

`soundAssetIdentifier`  

A name that refers to the audio data that the node plays. See assetIdentifier.

`mixerDefinition`  

An object that combines audio layers.

## See Also

### Creating a Sampler Node

convenience init(soundAssetIdentifier: String, mixerDefinition: PHASEMixerDefinition, identifier: String)

Creates a named sampler node with the given sound asset and mixer.

