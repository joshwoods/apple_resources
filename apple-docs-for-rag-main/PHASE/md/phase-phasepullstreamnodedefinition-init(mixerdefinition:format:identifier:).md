

- PHASE
- PHASEPullStreamNodeDefinition
-  init(mixerDefinition:format:identifier:) 

Initializer

# init(mixerDefinition:format:identifier:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
convenience init(
    mixerDefinition: PHASEMixerDefinition,
    format: AVAudioFormat,
    identifier: String
)
```

## Discussion

```
@method initWithMixerDefinition:format:identifier
@abstract Create a pull stream node definition
@param mixerDefinition
    The mixer definition this stream will be assigned to
@param format
    The AVAudioFormat object that will define the attributes of the audio this node will accept.
    Only Core Audio's standard deinterleaved 32-bit floating-point formats are supported.
@param identifier
    An optional custom identifier to give to this object
@return
    A new PHASEPullStreamNodeDefinition object
```

