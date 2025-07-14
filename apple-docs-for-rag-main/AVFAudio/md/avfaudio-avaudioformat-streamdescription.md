

- AVFAudio
- AVAudioFormat
-  streamDescription 

Instance Property

# streamDescription

The audio format properties of a stream of audio data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var streamDescription: UnsafePointer { get }
```

## Discussion

Returns an AudioStreamBasicDescription that you use with lower-level audio APIs.

