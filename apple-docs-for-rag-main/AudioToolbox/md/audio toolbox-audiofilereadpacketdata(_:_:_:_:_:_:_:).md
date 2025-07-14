

- Audio Toolbox
-  AudioFileReadPacketData(\_:\_:\_:\_:\_:\_:\_:) 

Function

# AudioFileReadPacketData(\_:\_:\_:\_:\_:\_:\_:)

Reads packets of audio data from an audio file.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileReadPacketData(
    _ inAudioFile: AudioFileID,
    _ inUseCache: Bool,
    _ ioNumBytes: UnsafeMutablePointer,
    _ outPacketDescriptions: UnsafeMutablePointer?,
    _ inStartingPacket: Int64,
    _ ioNumPackets: UnsafeMutablePointer,
    _ outBuffer: UnsafeMutableRawPointer?
) -> OSStatus
```

## Parameters 

`inAudioFile`  

The audio file whose audio packets you want to read.

`inUseCache`  

Set to `true` to cache the data. Otherwise, set to `false`.

`ioNumBytes`  

On input, the size of the `outBuffer` parameter, in bytes. On output, the number of bytes actually read.

You will see a difference in the input and output values if the byte size for the number of packets you request in the `ioNumPackets` parameter is smaller than the buffer size you pass in the `outBuffer` parameter. In this case, the output value for this parameter is smaller than its input value.

`outPacketDescriptions`  

On output, an array of packet descriptions for the packets that were read. The array that you pass in this parameter must be large enough to accommodate descriptions for the number of packets requested in the `ioNumPackets` parameter.

This parameter applies only to variable bit-rate data. If the file being read contains constant bit-rate (CBR) data, such as linear PCM, this parameter does not get filled. Pass `NULL` if the file’s data format is CBR.

`inStartingPacket`  

The packet index of the first packet you want to read.

`ioNumPackets`  

On input, the number of packets to read. On output, the number of packets actually read.

`outBuffer`  

Memory that you allocate to hold the read packets. Determine an appropriate size by multiplying the number of packets requested (in the `ioNumPackets` parameter) by the typical packet size for the audio data in the file. For uncompressed audio formats, a packet is equal to a frame.

## Return Value

A result code. See Result Codes.

## Discussion

Using this function is memory efficient when reading variable bit-rate (VBR) audio data, whose packet sizes can vary for a given duration of sound.

If the buffer you provide in the `outBuffer` parameter is too small to hold the packets you request in `ioNumPackets`, the output values of `ioNumPackets` and `ioNumBytes` are reduced to reflect the packets that were placed into the buffer. You also see a difference in the input and output values for `ioNumPackets` when this function has reached the end of the file you are reading. In this case, the output value for this parameter is smaller than its input value.

This function is more efficient than AudioFileReadPackets(_:_:_:_:_:_:_:) when reading compressed file formats that do not have packet tables, such as MP3 or ADTS. This function is a good choice for reading either CBR (constant bit-rate) or VBR data if you do not need to read a fixed duration of audio. If you do need to read a fixed duration of audio, whether CBR or VBR, use AudioFileReadPackets(_:_:_:_:_:_:_:) instead.

Audio File Services reads one 32-bit chunk of a file at a time.

## See Also

### Reading and Writing Audio Files

func AudioFileReadBytes(AudioFileID, Bool, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Reads bytes of audio data from an audio file.

func AudioFileWriteBytes(AudioFileID, Bool, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeRawPointer) -> OSStatus

Writes bytes of audio data to an audio file.

func AudioFileWritePackets(AudioFileID, Bool, UInt32, UnsafePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeRawPointer) -> OSStatus

Writes packets of audio data to an audio data file.

