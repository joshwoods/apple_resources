

- Audio Toolbox
-  AudioFileGetPropertyInfo(\_:\_:\_:\_:) 

Function

# AudioFileGetPropertyInfo(\_:\_:\_:\_:)

Gets information about an audio file property, including the size of the property value and whether the value is writable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileGetPropertyInfo(
    _ inAudioFile: AudioFileID,
    _ inPropertyID: AudioFilePropertyID,
    _ outDataSize: UnsafeMutablePointer?,
    _ isWritable: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`inAudioFile`  

The audio file you want to obtain property value information from.

`inPropertyID`  

The property whose value information you want. See Audio File Properties for possible values.

`outDataSize`  

On output, the size in bytes of the property value.

`isWritable`  

On output, equals `1` if the property is writable, or `0` if it is read-only.

## Return Value

A result code. See Result Codes.

## See Also

### Getting and Setting Audio File Properties

func AudioFileGetProperty(AudioFileID, AudioFilePropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Gets the value of an audio file property.

func AudioFileSetProperty(AudioFileID, AudioFilePropertyID, UInt32, UnsafeRawPointer) -> OSStatus

Sets the value of an audio file property

