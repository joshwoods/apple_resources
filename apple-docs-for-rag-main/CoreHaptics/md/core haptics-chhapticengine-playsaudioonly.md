

- Core Haptics
- CHHapticEngine
-  playsAudioOnly 

Instance Property

# playsAudioOnly

A Boolean value that indicates whether the engine ignores haptic events and plays audio events only.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var playsAudioOnly: Bool { get set }
```

## Discussion

If you set a new value on a running engine, you must restart the engine for the change to take effect.

The default value is false.

## See Also

### Modifying Playback Properties

var playsHapticsOnly: Bool

A Boolean value that indicates whether the engine ignores audio events.

var isMutedForAudio: Bool

A Boolean value that indicates whether the engine mutes audio.

var isMutedForHaptics: Bool

A Boolean value that indicates whether the engine mutes haptics.

