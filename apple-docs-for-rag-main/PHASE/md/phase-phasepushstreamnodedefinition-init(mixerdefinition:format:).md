

- PHASE
- PHASEPushStreamNodeDefinition
-  init(mixerDefinition:format:) 

Initializer

# init(mixerDefinition:format:)

Creates a node definition for audio streams.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
init(
    mixerDefinition: PHASEMixerDefinition,
    format: AVAudioFormat
)
```

## Parameters 

`mixerDefinition`  

An object that combines audio layers.

`format`  

The format of the audio stream data.

## See Also

### Creating a Node

convenience init(mixerDefinition: PHASEMixerDefinition, format: AVAudioFormat, identifier: String)

Creates a named node definition for audio streams.

