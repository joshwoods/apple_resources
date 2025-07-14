

- Audio Toolbox
-  AudioFileGetProperty(\_:\_:\_:\_:) 

Function

# AudioFileGetProperty(\_:\_:\_:\_:)

Gets the value of an audio file property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileGetProperty(
    _ inAudioFile: AudioFileID,
    _ inPropertyID: AudioFilePropertyID,
    _ ioDataSize: UnsafeMutablePointer,
    _ outPropertyData: UnsafeMutableRawPointer
) -> OSStatus
```

## Parameters 

`inAudioFile`  

The audio file you want to obtain a property value from.

`inPropertyID`  

The property whose value you want. See Audio File Properties for possible values.

`ioDataSize`  

On input, the size of the buffer passed in the `outPropertyData` parameter. On output, the number of bytes written to the buffer. Use the AudioFileGetPropertyInfo(_:_:_:_:) function to obtain the size of the property value.

`outPropertyData`  

On output, the value of the property specified in the `inPropertyID` parameter.

## Return Value

A result code. See Result Codes.

## Discussion

Some Core Audio property values are C types and others are Core Foundation objects.

If you call this function to retrieve a value that is a Core Foundation object, then this function—despite the use of “Get” in its name—duplicates the object. You are responsible for releasing the object, as described in The Create Rule in Memory Management Programming Guide for Core Foundation.

## See Also

### Getting and Setting Audio File Properties

func AudioFileGetPropertyInfo(AudioFileID, AudioFilePropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

Gets information about an audio file property, including the size of the property value and whether the value is writable.

func AudioFileSetProperty(AudioFileID, AudioFilePropertyID, UInt32, UnsafeRawPointer) -> OSStatus

Sets the value of an audio file property

