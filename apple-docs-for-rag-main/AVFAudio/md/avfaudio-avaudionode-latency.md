

- AVFAudio
- AVAudioNode
-  latency 

Instance Property

# latency

The processing latency of the node, in seconds.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var latency: TimeInterval { get }
```

## Discussion

This latency reflects the delay due to signal processing. A value of `0` indicates either no latency or an unknown latency.

## See Also

### Getting Audio Node Properties

var auAudioUnit: AUAudioUnit

An audio unit object that wraps or underlies the implementation’s audio unit.

var outputPresentationLatency: TimeInterval

The maximum render pipeline latency downstream of the node, in seconds.

