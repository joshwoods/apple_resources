

- Core Haptics
-  CHHapticAudioResourceKeyUseVolumeEnvelope 

Global Variable

# CHHapticAudioResourceKeyUseVolumeEnvelope

A key for a Boolean value that indicates whether audio file playback fades in and out using an envelope.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
let CHHapticAudioResourceKeyUseVolumeEnvelope: String
```

## Discussion

Fading, or ramping, the volume of an audio resource can prevent clicks during playback. It’s also useful in cases where the app modulates the envelope to use different attack and release times.

The default value is true.

## See Also

### Audio Resource Keys

let CHHapticAudioResourceKeyLoopEnabled: String

A key for a Boolean value that indicates whether to loop audio playback.

typealias CHHapticAudioResourceKey

A type alias for a key that identifies the playback behavior of an audio resource.

