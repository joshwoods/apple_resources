

- AVFAudio
- AVAudioTime
-  isSampleTimeValid 

Instance Property

# isSampleTimeValid

A Boolean value that indicates whether the sample time and sample rate properties are in a valid state.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isSampleTimeValid: Bool { get }
```

## See Also

### Getting Sample Rate Information

var sampleRate: Double

The sampling rate that the sample time property expresses.

var sampleTime: AVAudioFramePosition

The time as a number of audio samples that the current audio device tracks.

