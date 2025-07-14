

- PHASE
- PHASEPushStreamNode
-  mixer 

Instance Property

# mixer

The audio stream’s output pipeline.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var mixer: PHASEMixer { get }
```

## Discussion

The framework sets the value based on the definition initializer’s `mixerDefinition` argument. See init(mixerDefinition:format:).

## See Also

### Inspecting Stream Properties

var format: AVAudioFormat

The format of the audio stream data.

