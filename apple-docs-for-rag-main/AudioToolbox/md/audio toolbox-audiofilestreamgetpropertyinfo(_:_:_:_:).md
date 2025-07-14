

- Audio Toolbox
-  AudioFileStreamGetPropertyInfo(\_:\_:\_:\_:) 

Function

# AudioFileStreamGetPropertyInfo(\_:\_:\_:\_:)

Retrieves information about a property value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileStreamGetPropertyInfo(
    _ inAudioFileStream: AudioFileStreamID,
    _ inPropertyID: AudioFileStreamPropertyID,
    _ outPropertyDataSize: UnsafeMutablePointer?,
    _ outWritable: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`inAudioFileStream`  

The ID of the parser from which you wish to obtain information. The parser ID is returned by the AudioFileStreamOpen(_:_:_:_:_:) function.

`inPropertyID`  

A four-character ID indicating the audio file stream property about which you want information. See Audio File Stream Properties for possible values.

`outPropertyDataSize`  

On output, the size, in bytes, of the current value of the specified property.

`outWritable`  

On output, `true` if the property can be written. Currently, there are no writable audio file stream properties.

## Return Value

A result code. See Result Codes.

## See Also

### Related Documentation

func AudioFileStreamOpen(UnsafeMutableRawPointer?, AudioFileStream_PropertyListenerProc, AudioFileStream_PacketsProc, AudioFileTypeID, UnsafeMutablePointer&lt;AudioFileStreamID?>) -> OSStatus

Creates and opens a new audio file stream parser.

### Working with Data Stream Property Information

func AudioFileStreamGetProperty(AudioFileStreamID, AudioFileStreamPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Retrieves the value of the specified property.

func AudioFileStreamSetProperty(AudioFileStreamID, AudioFileStreamPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

Sets the value of the specified property.

