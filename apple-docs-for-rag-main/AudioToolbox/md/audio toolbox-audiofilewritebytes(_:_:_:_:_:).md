

- Audio Toolbox
-  AudioFileWriteBytes(\_:\_:\_:\_:\_:) 

Function

# AudioFileWriteBytes(\_:\_:\_:\_:\_:)

Writes bytes of audio data to an audio file.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileWriteBytes(
    _ inAudioFile: AudioFileID,
    _ inUseCache: Bool,
    _ inStartingByte: Int64,
    _ ioNumBytes: UnsafeMutablePointer,
    _ inBuffer: UnsafeRawPointer
) -> OSStatus
```

## Parameters 

`inAudioFile`  

The audio file to which you want to write bytes of data.

`inUseCache`  

Set to `true` if you want to cache the data. Otherwise, set to `false`.

`inStartingByte`  

The byte offset where the audio data should be written.

`ioNumBytes`  

On input, a pointer the number of bytes to write. On output, a pointer to the number of bytes actually written.

`inBuffer`  

A pointer to a buffer containing the bytes to be written.

## Return Value

A result code. See Result Codes.

## Discussion

In most cases, you should use AudioFileWritePackets(_:_:_:_:_:_:_:) instead of this function.

## See Also

### Reading and Writing Audio Files

func AudioFileReadBytes(AudioFileID, Bool, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Reads bytes of audio data from an audio file.

func AudioFileReadPacketData(AudioFileID, Bool, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer?) -> OSStatus

Reads packets of audio data from an audio file.

func AudioFileWritePackets(AudioFileID, Bool, UInt32, UnsafePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeRawPointer) -> OSStatus

Writes packets of audio data to an audio data file.

