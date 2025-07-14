

- AVFAudio
- AVAudioRecorder
-  updateMeters() 

Instance Method

# updateMeters()

Refreshes the average and peak power values for all channels of an audio recorder.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+tvOS 17.0+visionOS 1.0+watchOS 4.0+

``` source
func updateMeters()
```

## Discussion

Call this method to update the level meter data before calling averagePower(forChannel:) or peakPower(forChannel:).

## See Also

### Managing audio-level metering

var isMeteringEnabled: Bool

A Boolean value that indicates whether you’ve enabled the recorder to generate audio-level metering data.

func averagePower(forChannel: Int) -> Float

Returns the average power, in decibels full-scale (dBFS), for an audio channel.

func peakPower(forChannel: Int) -> Float

Returns the peak power, in decibels full-scale (dBFS), for an audio channel.

