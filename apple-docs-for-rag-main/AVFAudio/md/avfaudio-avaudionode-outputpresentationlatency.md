

- AVFAudio
- AVAudioNode
-  outputPresentationLatency 

Instance Property

# outputPresentationLatency

The maximum render pipeline latency downstream of the node, in seconds.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var outputPresentationLatency: TimeInterval { get }
```

## Discussion

This latency describes the maximum time it takes to present the audio at the output of a node.

## See Also

### Getting Audio Node Properties

var auAudioUnit: AUAudioUnit

An audio unit object that wraps or underlies the implementation’s audio unit.

var latency: TimeInterval

The processing latency of the node, in seconds.

