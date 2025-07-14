

- AVFAudio
- AVAudioPlayer
-  averagePower(forChannel:) 

Instance Method

# averagePower(forChannel:)

Returns the average power, in decibels full-scale (dBFS), for an audio channel.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func averagePower(forChannel channelNumber: Int) -> Float
```

## Parameters 

`channelNumber`  

The audio channel with the average power value you want to retrieve. Channel numbers are zero-indexed. A monaural signal, or the left channel of a stereo signal, has channel number `0`.

## Return Value

A floating-point value, in dBFS, that indicates the audio channel’s current average power.

## Discussion

Before asking the player for its average power value, you must call updateMeters() to generate the latest data. The returned value ranges from `–160` dBFS, indicating minimum power, to 0 dBFS, indicating maximum power.

## See Also

### Managing audio-level metering

var isMeteringEnabled: Bool

A Boolean value that indicates whether the player is able to generate audio-level metering data.

func updateMeters()

Refreshes the average and peak power values for all channels of an audio player.

func peakPower(forChannel: Int) -> Float

Returns the peak power, in decibels full-scale (dBFS), for an audio channel.

