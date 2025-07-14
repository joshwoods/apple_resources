

- Audio Toolbox
-  AudioFileSetProperty(\_:\_:\_:\_:) 

Function

# AudioFileSetProperty(\_:\_:\_:\_:)

Sets the value of an audio file property

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileSetProperty(
    _ inAudioFile: AudioFileID,
    _ inPropertyID: AudioFilePropertyID,
    _ inDataSize: UInt32,
    _ inPropertyData: UnsafeRawPointer
) -> OSStatus
```

## Parameters 

`inAudioFile`  

The audio file that you want to set a property value for.

`inPropertyID`  

The property whose value you want to set. See Audio File Properties for possible values. Use the AudioFileGetPropertyInfo(_:_:_:_:) function to determine whether the property value is writable.

`inDataSize`  

The size of the value you are passing in the `inPropertyData` parameter.

`inPropertyData`  

The new value for the property.

## Return Value

A result code. See Result Codes.

## See Also

### Getting and Setting Audio File Properties

func AudioFileGetProperty(AudioFileID, AudioFilePropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Gets the value of an audio file property.

func AudioFileGetPropertyInfo(AudioFileID, AudioFilePropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

Gets information about an audio file property, including the size of the property value and whether the value is writable.

