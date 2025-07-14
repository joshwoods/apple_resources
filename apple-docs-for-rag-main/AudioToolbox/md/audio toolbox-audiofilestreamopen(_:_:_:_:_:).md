

- Audio Toolbox
-  AudioFileStreamOpen(\_:\_:\_:\_:\_:) 

Function

# AudioFileStreamOpen(\_:\_:\_:\_:\_:)

Creates and opens a new audio file stream parser.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileStreamOpen(
    _ inClientData: UnsafeMutableRawPointer?,
    _ inPropertyListenerProc: AudioFileStream_PropertyListenerProc,
    _ inPacketsProc: AudioFileStream_PacketsProc,
    _ inFileTypeHint: AudioFileTypeID,
    _ outAudioFileStream: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inClientData`  

A pointer to a value or structure to be passed to your callback functions.

`inPropertyListenerProc`  

Your property-listener callback. Whenever the parser finds the value of a property in the data stream, it calls your property listener with the property ID. You can then call the AudioFileStreamGetPropertyInfo(_:_:_:_:) and AudioFileStreamGetProperty(_:_:_:_:) functions to get the value of the property.

`inPacketsProc`  

Your audio-data callback. Whenever the parser finds audio data packets in the data stream, it passes the data to your audio-data callback.

`inFileTypeHint`  

An audio file type hint. If the audio file stream that you intend to pass to the parser is of a type that the parser cannot easily or uniquely determine from the data (such as ADTS or AC3), you can use this parameter to indicate the type. Possible values are listed in the AudioFileTypeID enumeration in Audio File Services.

If you do not know the audio file type, pass `0`.

`outAudioFileStream`  

On output, an opaque object representing the audio file stream parser. This object is referred to in this document as the audio file stream parser ID. You need to pass this ID in to other functions in the Audio File Stream API.

## Return Value

A result code. See Result Codes.

## See Also

### Related Documentation

func AudioFileStreamGetPropertyInfo(AudioFileStreamID, AudioFileStreamPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Retrieves information about a property value.

typealias AudioFileStream_PropertyListenerProc

Invoked by an audio file stream parser when it finds a property value in the audio file stream.

func AudioFileStreamGetProperty(AudioFileStreamID, AudioFileStreamPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Retrieves the value of the specified property.

typealias AudioFileStream_PacketsProc

Invoked by an audio file stream parser when it finds audio data in the audio file stream.

