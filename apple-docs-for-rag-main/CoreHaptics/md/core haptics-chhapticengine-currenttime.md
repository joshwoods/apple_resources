

- Core Haptics
- CHHapticEngine
-  currentTime 

Instance Property

# currentTime

The absolute time, in seconds, to use for scheduling haptic and audio events.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var currentTime: TimeInterval { get }
```

## Discussion

This time applies to all haptic and audio events sent to and managed by the Core Haptics engine. Use the current time as a way to determine or track the start times of haptic and audio events, created as CHHapticEvent objects. It corresponds to the relativeTime and duration properties of haptic events.

Note

The Core Haptics engine time doesn’t correlate to time used in media playback classes from other frameworks, such as AVAudioPlayer.

## See Also

### Getting the Current Media Time

var CHHapticTimeImmediate: TimeInterval

A time constant used to schedule a command immediately.

