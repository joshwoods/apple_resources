

- PHASE
- PHASEChannelMixerDefinition
-  init(channelLayout:identifier:) 

Initializer

# init(channelLayout:identifier:)

Creates a named channel mixer with the given channel layout.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
convenience init(
    channelLayout layout: AVAudioChannelLayout,
    identifier: String
)
```

## Parameters 

`layout`  

A channel configuration for the mixer’s input audio.

`identifier`  

A unique name for the channel mixer.

## See Also

### Creating a Channel Mixer

init(channelLayout: AVAudioChannelLayout)

Creates a channel mixer with the given channel layout.

