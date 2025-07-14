

- AVFAudio
- AVAudioNode
-  auAudioUnit 

Instance Property

# auAudioUnit

An audio unit object that wraps or underlies the implementation’s audio unit.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var auAudioUnit: AUAudioUnit { get }
```

## Discussion

This provides an AUAudioUnit that either wraps or underlies the implementation’s audio unit, depending on how the app packages the audio unit. Apps interact with this to control custom properties, select presets, and change parameters.

Don’t perform operations directly on the audio unit that may conflict with the engine’s state, which includes changing the initialization state, stream formats, channel layouts, or connections to other audio units.

## See Also

### Getting Audio Node Properties

var latency: TimeInterval

The processing latency of the node, in seconds.

var outputPresentationLatency: TimeInterval

The maximum render pipeline latency downstream of the node, in seconds.

