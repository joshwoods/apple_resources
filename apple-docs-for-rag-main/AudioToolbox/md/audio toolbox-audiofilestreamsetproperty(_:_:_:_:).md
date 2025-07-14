

- Audio Toolbox
-  AudioFileStreamSetProperty(\_:\_:\_:\_:) 

Function

# AudioFileStreamSetProperty(\_:\_:\_:\_:)

Sets the value of the specified property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileStreamSetProperty(
    _ inAudioFileStream: AudioFileStreamID,
    _ inPropertyID: AudioFileStreamPropertyID,
    _ inPropertyDataSize: UInt32,
    _ inPropertyData: UnsafeRawPointer
) -> OSStatus
```

## Parameters 

`inAudioFileStream`  

The ID of the parser to which you wish to pass data. The parser ID is returned by the AudioFileStreamOpen(_:_:_:_:_:) function.

`inPropertyID`  

The ID of the audio file stream property whose value is to be set.

`inPropertyDataSize`  

The size, in bytes, of the property data.

`inPropertyData`  

The property data.

## Return Value

A result code. See Result Codes.

## Discussion

Currently, there are no settable properties.

## See Also

### Related Documentation

func AudioFileStreamOpen(UnsafeMutableRawPointer?, AudioFileStream_PropertyListenerProc, AudioFileStream_PacketsProc, AudioFileTypeID, UnsafeMutablePointer&lt;AudioFileStreamID?>) -> OSStatus

Creates and opens a new audio file stream parser.

### Working with Data Stream Property Information

func AudioFileStreamGetPropertyInfo(AudioFileStreamID, AudioFileStreamPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Retrieves information about a property value.

func AudioFileStreamGetProperty(AudioFileStreamID, AudioFileStreamPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Retrieves the value of the specified property.

