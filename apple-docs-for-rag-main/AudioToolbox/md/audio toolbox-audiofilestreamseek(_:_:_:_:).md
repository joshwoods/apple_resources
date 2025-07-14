

- Audio Toolbox
-  AudioFileStreamSeek(\_:\_:\_:\_:) 

Function

# AudioFileStreamSeek(\_:\_:\_:\_:)

Provides a byte offset for a specified packet in the data stream.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileStreamSeek(
    _ inAudioFileStream: AudioFileStreamID,
    _ inPacketOffset: Int64,
    _ outDataByteOffset: UnsafeMutablePointer,
    _ ioFlags: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inAudioFileStream`  

The ID of the parser to which you wish to provide a byte offset. The parser ID is returned by the AudioFileStreamOpen(_:_:_:_:_:) function.

`inPacketOffset`  

The number of packets from the beginning of the file of the packet whose byte offset you wish to have returned.

`outDataByteOffset`  

On output, the absolute byte offset of the packet whose offset you specify in the `inPacketOffset` parameter. For audio file formats that do not contain packet tables, the returned offset may be an estimate.

`ioFlags`  

On output, if the `outDataByteOffset` parameter returns an estimate, this parameter returns the constant `kAudioFileStreamSeekFlag_OffsetIsEstimated`. Currently, no input flags are defined for this call.

## Return Value

A result code. See Result Codes.

## Discussion

After you call this function, the parser assumes the next data passed to the AudioFileStreamParseBytes(_:_:_:_:) function starts from the byte offset returned in the `outDataByteOffset` parameter.

## See Also

### Related Documentation

func AudioFileStreamParseBytes(AudioFileStreamID, UInt32, UnsafeRawPointer?, AudioFileStreamParseFlags) -> OSStatus

Passes audio file stream data to the parser.

func AudioFileStreamOpen(UnsafeMutableRawPointer?, AudioFileStream_PropertyListenerProc, AudioFileStream_PacketsProc, AudioFileTypeID, UnsafeMutablePointer&lt;AudioFileStreamID?>) -> OSStatus

Creates and opens a new audio file stream parser.

