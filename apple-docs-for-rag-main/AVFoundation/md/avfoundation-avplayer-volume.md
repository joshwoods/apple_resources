

- AVFoundation
- AVPlayer
-  volume 

Instance Property

# volume

The audio playback volume for the player.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
var volume: Float { get set }
```

## Discussion

A value of `0.0` indicates silence; a value of `1.0` (the default) indicates full audio volume for the player instance.

This property is used to control the player audio volume relative to the system volume. There is no programmatic way to control the system volume in iOS, but you can use the MediaPlayer framework’s MPVolumeView class to present a standard user interface for controlling system volume.

## See Also

### Configuring Audio Behavior

var isMuted: Bool

A Boolean value that indicates whether the audio output of the player is muted.

var allowedAudioSpatializationFormats: AVAudioSpatializationFormats

The source audio channel layouts the player item supports for spatialization.

var isAudioSpatializationAllowed: Bool

A Boolean value that indicates whether the player item allows spatialized audio playback.

Deprecated

