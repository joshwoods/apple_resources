

- AVFAudio
- AVAudioFormat
-  isEqual(\_:) 

Instance Method

# isEqual(\_:)

Indicates whether the audio format instance and a specified object are functionally equivalent.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isEqual(_ object: Any) -> Bool
```

## Parameters 

`object`  

The object to compare.

## Return Value

A Boolean value of true if the receiver and `object` are equal; otherwise, false.

## Discussion

The PCM format ignores interleaveness for mono.

The method ignores the differences in the AudioStreamBasicDescription alignment and packedness when they’re not significant. For example, with one channel, 2 bytes per frame, 16 bits per channel, and neither alignment, the format is implicit packedness and the method can interpret it as either high- or low-aligned.

For AVAudioChannelLayout, the method considers a layout with the standard mono or stereo tag to be equivalent to a `nil` layout.

Otherwise, the method compares the layouts for equality.

