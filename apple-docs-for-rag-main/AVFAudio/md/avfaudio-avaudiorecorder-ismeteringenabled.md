

- AVFAudio
- AVAudioRecorder
-  isMeteringEnabled 

Instance Property

# isMeteringEnabled

A Boolean value that indicates whether you’ve enabled the recorder to generate audio-level metering data.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+tvOS 17.0+visionOS 1.0+watchOS 4.0+

``` source
var isMeteringEnabled: Bool { get set }
```

## Discussion

By default, the recorder doesn’t generate audio-level metering data. Because metering uses computing resources, enable it only if you intend to use it.

## See Also

### Managing audio-level metering

func updateMeters()

Refreshes the average and peak power values for all channels of an audio recorder.

func averagePower(forChannel: Int) -> Float

Returns the average power, in decibels full-scale (dBFS), for an audio channel.

func peakPower(forChannel: Int) -> Float

Returns the peak power, in decibels full-scale (dBFS), for an audio channel.

