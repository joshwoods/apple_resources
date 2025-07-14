

- AVFAudio
- AVAudioRecorder
-  averagePower(forChannel:) 

Instance Method

# averagePower(forChannel:)

Returns the average power, in decibels full-scale (dBFS), for an audio channel.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+tvOS 17.0+visionOS 1.0+watchOS 4.0+

``` source
func averagePower(forChannel channelNumber: Int) -> Float
```

## Parameters 

`channelNumber`  

The number of the channel that you want the average power value for.

## Return Value

The audio channel’s current average power.

## Discussion

Before asking the player for its average power value, you must call updateMeters() to generate the latest data. The returned value ranges from `–160` dBFS, indicating minimum power, to 0 dBFS, indicating maximum power.

## See Also

### Managing audio-level metering

var isMeteringEnabled: Bool

A Boolean value that indicates whether you’ve enabled the recorder to generate audio-level metering data.

func updateMeters()

Refreshes the average and peak power values for all channels of an audio recorder.

func peakPower(forChannel: Int) -> Float

Returns the peak power, in decibels full-scale (dBFS), for an audio channel.

