

- Core Haptics
- CHHapticEngine
-  playsHapticsOnly 

Instance Property

# playsHapticsOnly

A Boolean value that indicates whether the engine ignores audio events.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var playsHapticsOnly: Bool { get set }
```

## Discussion

Setting this property to true causes the engine to ignore all audio events, such as audioContinuous and audioCustom. This also reduces latency of starting haptic playback.

Important

Changing the value of this property on a running engine has no effect until you stop and restart the engine.

## See Also

### Modifying Playback Properties

var playsAudioOnly: Bool

A Boolean value that indicates whether the engine ignores haptic events and plays audio events only.

var isMutedForAudio: Bool

A Boolean value that indicates whether the engine mutes audio.

var isMutedForHaptics: Bool

A Boolean value that indicates whether the engine mutes haptics.

