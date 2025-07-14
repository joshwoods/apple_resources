

- Audio Toolbox
-  ExtAudioFileSetProperty(\_:\_:\_:\_:) 

Function

# ExtAudioFileSetProperty(\_:\_:\_:\_:)

Sets a property value for an extended audio file object.

iOS 2.1+iPadOS 2.1+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func ExtAudioFileSetProperty(
    _ inExtAudioFile: ExtAudioFileRef,
    _ inPropertyID: ExtAudioFilePropertyID,
    _ inPropertyDataSize: UInt32,
    _ inPropertyData: UnsafeRawPointer
) -> OSStatus
```

## Parameters 

`inExtAudioFile`  

The extended audio file object to set a property value on.

`inPropertyID`  

The property whose value you want to set.

`inPropertyDataSize`  

The size of the property value, in bytes.

`inPropertyData`  

The value you want to apply to the specified property.

## Return Value

A result code.

## See Also

### Configuring Properties for Extended Audio File Objects

func ExtAudioFileGetProperty(ExtAudioFileRef, ExtAudioFilePropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Gets a property value from an extended audio file object.

func ExtAudioFileGetPropertyInfo(ExtAudioFileRef, ExtAudioFilePropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets information about an extended audio file object property.

