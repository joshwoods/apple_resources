

- PHASE
- PHASEPullStreamNodeDefinition
-  init(mixerDefinition:format:) 

Initializer

# init(mixerDefinition:format:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
init(
    mixerDefinition: PHASEMixerDefinition,
    format: AVAudioFormat
)
```

## Discussion

```
@method initWithMixerDefinition:format
@abstract Create a pull stream node definition
@param mixerDefinition
    The mixer definition this stream will be assigned to
@param format
    The AVAudioFormat object that will define the attributes of the audio this node will accept.
    Only Core Audio's standard deinterleaved 32-bit floating-point formats are supported.
@return
    A new PHASEPullStreamNodeDefinition object
```

