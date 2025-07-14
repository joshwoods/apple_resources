

- AVFAudio
- AVAudioTime
-  init(hostTime:) 

Initializer

# init(hostTime:)

Creates an audio time object with the specified host time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(hostTime: UInt64)
```

## Parameters 

`hostTime`  

The host time.

## Return Value

A new AVAudioTime instance.

## See Also

### Creating an Audio Time Instance

init(audioTimeStamp: UnsafePointer&lt;AudioTimeStamp>, sampleRate: Double)

Creates an audio time object with the specified timestamp and sample rate.

init(hostTime: UInt64, sampleTime: AVAudioFramePosition, atRate: Double)

Creates an audio time object with the specified host time, sample time, and sample rate.

init(sampleTime: AVAudioFramePosition, atRate: Double)

Creates an audio time object with the specified timestamp and sample rate.

func extrapolateTime(fromAnchor: AVAudioTime) -> AVAudioTime?

Creates an audio time object by converting between host time and sample time.

