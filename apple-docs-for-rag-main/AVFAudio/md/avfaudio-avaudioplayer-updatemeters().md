

- AVFAudio
- AVAudioPlayer
-  updateMeters() 

Instance Method

# updateMeters()

Refreshes the average and peak power values for all channels of an audio player.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func updateMeters()
```

## See Also

### Managing audio-level metering

var isMeteringEnabled: Bool

A Boolean value that indicates whether the player is able to generate audio-level metering data.

func averagePower(forChannel: Int) -> Float

Returns the average power, in decibels full-scale (dBFS), for an audio channel.

func peakPower(forChannel: Int) -> Float

Returns the peak power, in decibels full-scale (dBFS), for an audio channel.

