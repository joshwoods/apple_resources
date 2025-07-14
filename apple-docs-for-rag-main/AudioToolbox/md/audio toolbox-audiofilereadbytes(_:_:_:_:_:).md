

- Audio Toolbox
-  AudioFileReadBytes(\_:\_:\_:\_:\_:) 

Function

# AudioFileReadBytes(\_:\_:\_:\_:\_:)

Reads bytes of audio data from an audio file.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileReadBytes(
    _ inAudioFile: AudioFileID,
    _ inUseCache: Bool,
    _ inStartingByte: Int64,
    _ ioNumBytes: UnsafeMutablePointer,
    _ outBuffer: UnsafeMutableRawPointer
) -> OSStatus
```

## Parameters 

`inAudioFile`  

The audio file whose bytes of audio data you want to read.

`inUseCache`  

Set to `true` if you want to cache the data. You should cache reads and writes if you read or write the same portion of a file multiple times. To request that the data not be cached, if possible, set to `false`. You should not cache reads and writes if you read or write data from a file only once.

`inStartingByte`  

The byte offset of the audio data you want to be returned.

`ioNumBytes`  

On input, a pointer to the number of bytes to read. On output, a pointer to the number of bytes actually read.

`outBuffer`  

A pointer to user-allocated memory large enough for the requested bytes.

## Return Value

A result code. See Result Codes.

## Discussion

In most cases, you should use AudioFileReadPackets(_:_:_:_:_:_:_:) instead of this function.

This function returns `eofErr` when the read operation encounters the end of the file. Note that Audio File Services only reads one 32-bit chunk of a file at a time.

## See Also

### Reading and Writing Audio Files

func AudioFileWriteBytes(AudioFileID, Bool, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeRawPointer) -> OSStatus

Writes bytes of audio data to an audio file.

func AudioFileReadPacketData(AudioFileID, Bool, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer?) -> OSStatus

Reads packets of audio data from an audio file.

func AudioFileWritePackets(AudioFileID, Bool, UInt32, UnsafePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeRawPointer) -> OSStatus

Writes packets of audio data to an audio data file.

