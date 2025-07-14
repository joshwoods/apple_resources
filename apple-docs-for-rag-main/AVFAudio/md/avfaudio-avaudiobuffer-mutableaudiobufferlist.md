

- AVFAudio
- AVAudioBuffer
-  mutableAudioBufferList 

Instance Property

# mutableAudioBufferList

A mutable version of the buffer’s underlying audio buffer list.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var mutableAudioBufferList: UnsafeMutablePointer { get }
```

## Discussion

You use this with some lower-level Core Audio and Audio Toolbox APIs that require a mutable AudioBufferList (for example, the AudioConverterConvertComplexBuffer(_:_:_:_:) function).

The `mDataByteSize` fields of this audio buffer list express the buffer’s current frameCapacity. If you alter the capacity, modify the buffer’s `frameLength` to match.

## See Also

### Getting the Audio Buffers

var audioBufferList: UnsafePointer&lt;AudioBufferList>

The buffer’s underlying audio buffer list.

