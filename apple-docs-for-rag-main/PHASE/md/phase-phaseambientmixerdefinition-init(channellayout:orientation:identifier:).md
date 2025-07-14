

- PHASE
- PHASEAmbientMixerDefinition
-  init(channelLayout:orientation:identifier:) 

Initializer

# init(channelLayout:orientation:identifier:)

Creates a named ambient mixer with the given channel layout and orientation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
convenience init(
    channelLayout layout: AVAudioChannelLayout,
    orientation: simd_quatf,
    identifier: String
)
```

## Parameters 

`layout`  

The channel layout of input audio.

`orientation`  

A quaternion that describes the orientation of the speaker layout relative to the scene origin.

`identifier`  

A unique name for the mixer.

## See Also

### Creating an Ambient Mixer

init(channelLayout: AVAudioChannelLayout, orientation: simd_quatf)

Creates an ambient mixer with the given channel layout and orientation.

