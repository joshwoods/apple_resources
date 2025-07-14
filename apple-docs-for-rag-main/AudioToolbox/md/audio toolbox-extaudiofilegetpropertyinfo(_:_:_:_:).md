

- Audio Toolbox
-  ExtAudioFileGetPropertyInfo(\_:\_:\_:\_:) 

Function

# ExtAudioFileGetPropertyInfo(\_:\_:\_:\_:)

Gets information about an extended audio file object property.

iOS 2.1+iPadOS 2.1+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func ExtAudioFileGetPropertyInfo(
    _ inExtAudioFile: ExtAudioFileRef,
    _ inPropertyID: ExtAudioFilePropertyID,
    _ outSize: UnsafeMutablePointer?,
    _ outWritable: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`inExtAudioFile`  

The extended audio file object to get property information from.

`inPropertyID`  

The property you want information about.

`outSize`  

On output, the size of the property value in bytes. Can be `NULL` on output.

`outWritable`  

On output, a Boolean value indicating whether the property value is writable (`true` means writable). Can be `NULL` on output.

## Return Value

A result code.

## See Also

### Configuring Properties for Extended Audio File Objects

func ExtAudioFileGetProperty(ExtAudioFileRef, ExtAudioFilePropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Gets a property value from an extended audio file object.

func ExtAudioFileSetProperty(ExtAudioFileRef, ExtAudioFilePropertyID, UInt32, UnsafeRawPointer) -> OSStatus

Sets a property value for an extended audio file object.

