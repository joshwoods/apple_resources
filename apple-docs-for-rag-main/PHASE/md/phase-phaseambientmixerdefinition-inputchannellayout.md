

- PHASE
- PHASEAmbientMixerDefinition
-  inputChannelLayout 

Instance Property

# inputChannelLayout

The channel layout of input audio.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var inputChannelLayout: AVAudioChannelLayout { get }
```

## Discussion

The framework sets the value to the `channelLayout` initializer argument. See init(channelLayout:orientation:).

## See Also

### Inspecting the Mixer

var orientation: simd_quatf

A quaternion that describes the orientation of the speaker layout relative to the scene origin.

