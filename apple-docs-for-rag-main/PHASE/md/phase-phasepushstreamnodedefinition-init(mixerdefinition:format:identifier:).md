

- PHASE
- PHASEPushStreamNodeDefinition
-  init(mixerDefinition:format:identifier:) 

Initializer

# init(mixerDefinition:format:identifier:)

Creates a named node definition for audio streams.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
convenience init(
    mixerDefinition: PHASEMixerDefinition,
    format: AVAudioFormat,
    identifier: String
)
```

## Parameters 

`mixerDefinition`  

An object that combines audio layers.

`format`  

The format of the audio stream data.

`identifier`  

A unique name for the node.

## See Also

### Creating a Node

init(mixerDefinition: PHASEMixerDefinition, format: AVAudioFormat)

Creates a node definition for audio streams.

