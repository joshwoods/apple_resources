

- AVFAudio
- AVAudioTime
-  extrapolateTime(fromAnchor:) 

Instance Method

# extrapolateTime(fromAnchor:)

Creates an audio time object by converting between host time and sample time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func extrapolateTime(fromAnchor anchorTime: AVAudioTime) -> AVAudioTime?
```

## Parameters 

`anchorTime`  

An audio time instance with a more complete timestamp than that of the receiver (self).

## Return Value

A new AVAudioTime instance.

## Discussion

If `anchorTime` is an `AVAudioTime` instance where both host time and sample time are valid, and the receiver is another timestamp where only one of the two is valid, this method returns a new `AVAudioTime`. It copies it from the receiver, where the anchor provides additional valid fields.

The `anchorTime` value must have a valid host time and sample time, and self must have sample rate and at least one valid host time or sample time. Otherwise, this method returns `nil`.

```
// time0 has a valid audio sample representation, but no host time representation.
AVAudioTime *time0 = [AVAudioTime timeWithSampleTime: 0.0 atRate: 44100.0];
// anchor has a valid host time representation and sample time representation.
AVAudioTime *anchor = [node currentTime];
// fill in  valid host time representation
AVAudioTime *fullTime = [sampleTime extrapolateTimeFromAnchor: sampleTime];
```

## See Also

### Creating an Audio Time Instance

init(audioTimeStamp: UnsafePointer&lt;AudioTimeStamp>, sampleRate: Double)

Creates an audio time object with the specified timestamp and sample rate.

init(hostTime: UInt64)

Creates an audio time object with the specified host time.

init(hostTime: UInt64, sampleTime: AVAudioFramePosition, atRate: Double)

Creates an audio time object with the specified host time, sample time, and sample rate.

init(sampleTime: AVAudioFramePosition, atRate: Double)

Creates an audio time object with the specified timestamp and sample rate.

