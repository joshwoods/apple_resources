

- AVFAudio
- AVAudioBuffer
-  audioBufferList 

Instance Property

# audioBufferList

The buffer’s underlying audio buffer list.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var audioBufferList: UnsafePointer { get }
```

## Discussion

A buffer list is a variable length array that contains an array of audio buffer instances. You use it with lower-level Core Audio and Audio Toolbox API.

You must not modify the buffer list structure, although you can modify buffer contents.

The `mDataByteSize` fields of this audio buffer list express the buffer’s current frameLength.

## See Also

### Getting the Audio Buffers

var mutableAudioBufferList: UnsafeMutablePointer&lt;AudioBufferList>

A mutable version of the buffer’s underlying audio buffer list.

