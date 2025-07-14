

- AVFAudio
- AVAudioTime
-  init(sampleTime:atRate:) 

Initializer

# init(sampleTime:atRate:)

Creates an audio time object with the specified timestamp and sample rate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    sampleTime: AVAudioFramePosition,
    atRate sampleRate: Double
)
```

## Parameters 

`sampleTime`  

The sample time.

`sampleRate`  

The sample rate.

## Return Value

A new AVAudioTime instance.

## See Also

### Creating an Audio Time Instance

init(audioTimeStamp: UnsafePointer&lt;AudioTimeStamp>, sampleRate: Double)

Creates an audio time object with the specified timestamp and sample rate.

init(hostTime: UInt64)

Creates an audio time object with the specified host time.

init(hostTime: UInt64, sampleTime: AVAudioFramePosition, atRate: Double)

Creates an audio time object with the specified host time, sample time, and sample rate.

func extrapolateTime(fromAnchor: AVAudioTime) -> AVAudioTime?

Creates an audio time object by converting between host time and sample time.

