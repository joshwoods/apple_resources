

- Audio Toolbox
-  AudioFileWritePackets(\_:\_:\_:\_:\_:\_:\_:) 

Function

# AudioFileWritePackets(\_:\_:\_:\_:\_:\_:\_:)

Writes packets of audio data to an audio data file.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileWritePackets(
    _ inAudioFile: AudioFileID,
    _ inUseCache: Bool,
    _ inNumBytes: UInt32,
    _ inPacketDescriptions: UnsafePointer?,
    _ inStartingPacket: Int64,
    _ ioNumPackets: UnsafeMutablePointer,
    _ inBuffer: UnsafeRawPointer
) -> OSStatus
```

## Parameters 

`inAudioFile`  

The audio file to write to.

`inUseCache`  

Set to `true` if you want to cache the data. Otherwise, set to `false`.

`inNumBytes`  

The number of bytes of audio data being written.

`inPacketDescriptions`  

A pointer to an array of packet descriptions for the audio data. Not all formats require packet descriptions. If no packet descriptions are required, for instance, if you are writing CBR data, pass `NULL`.

`inStartingPacket`  

The packet index for the placement of the first provided packet.

`ioNumPackets`  

On input, a pointer to the number of packets to write. On output, a pointer to the number of packets actually written.

`inBuffer`  

A pointer to user-allocated memory containing the new audio data to write to the audio data file.

## Return Value

A result code. See Result Codes.

## Discussion

For all uncompressed formats, this function equates packets with frames.

## See Also

### Related Documentation

func AudioFileReadPackets(AudioFileID, Bool, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer?) -> OSStatus

Reads a fixed duration of audio data from an audio file.

Deprecated

### Reading and Writing Audio Files

func AudioFileReadBytes(AudioFileID, Bool, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Reads bytes of audio data from an audio file.

func AudioFileWriteBytes(AudioFileID, Bool, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeRawPointer) -> OSStatus

Writes bytes of audio data to an audio file.

func AudioFileReadPacketData(AudioFileID, Bool, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer?) -> OSStatus

Reads packets of audio data from an audio file.

