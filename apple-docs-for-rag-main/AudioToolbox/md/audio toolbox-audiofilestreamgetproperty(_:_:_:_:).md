

- Audio Toolbox
-  AudioFileStreamGetProperty(\_:\_:\_:\_:) 

Function

# AudioFileStreamGetProperty(\_:\_:\_:\_:)

Retrieves the value of the specified property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileStreamGetProperty(
    _ inAudioFileStream: AudioFileStreamID,
    _ inPropertyID: AudioFileStreamPropertyID,
    _ ioPropertyDataSize: UnsafeMutablePointer,
    _ outPropertyData: UnsafeMutableRawPointer
) -> OSStatus
```

## Parameters 

`inAudioFileStream`  

The ID of the parser from which you wish to obtain data. The parser ID is returned by the AudioFileStreamOpen(_:_:_:_:_:) function.

`inPropertyID`  

A four-character ID indicating the audio file stream property whose value you want to read. See Audio File Stream Properties for possible values.

`ioPropertyDataSize`  

On input, the size of the buffer in the `outPropertyData` parameter. Call the AudioFileStreamGetPropertyInfo(_:_:_:_:) function to obtain the size of the property value. On output, the number of bytes of the property value returned.

`outPropertyData`  

On output, the value of the specified property.

## Return Value

A result code. See Result Codes.

## Discussion

Some Core Audio property values are C types and others are Core Foundation objects.

If you call this function to retrieve a value that is a Core Foundation object, then this function—despite the use of “Get” in its name—duplicates the object. You are responsible for releasing the object, as described in The Create Rule in Memory Management Programming Guide for Core Foundation.

## See Also

### Related Documentation

func AudioFileStreamOpen(UnsafeMutableRawPointer?, AudioFileStream_PropertyListenerProc, AudioFileStream_PacketsProc, AudioFileTypeID, UnsafeMutablePointer&lt;AudioFileStreamID?>) -> OSStatus

Creates and opens a new audio file stream parser.

### Working with Data Stream Property Information

func AudioFileStreamGetPropertyInfo(AudioFileStreamID, AudioFileStreamPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Retrieves information about a property value.

func AudioFileStreamSetProperty(AudioFileStreamID, AudioFileStreamPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

Sets the value of the specified property.

