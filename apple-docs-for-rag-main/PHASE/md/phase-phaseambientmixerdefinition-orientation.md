

- PHASE
- PHASEAmbientMixerDefinition
-  orientation 

Instance Property

# orientation

A quaternion that describes the orientation of the speaker layout relative to the scene origin.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var orientation: simd_quatf { get }
```

## Discussion

The framework sets the value to the `orientation` initializer argument. See init(channelLayout:orientation:).

## See Also

### Inspecting the Mixer

var inputChannelLayout: AVAudioChannelLayout

The channel layout of input audio.

