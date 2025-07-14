

- Audio Toolbox
-  ExtAudioFileGetProperty(\_:\_:\_:\_:) 

Function

# ExtAudioFileGetProperty(\_:\_:\_:\_:)

Gets a property value from an extended audio file object.

iOS 2.1+iPadOS 2.1+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func ExtAudioFileGetProperty(
    _ inExtAudioFile: ExtAudioFileRef,
    _ inPropertyID: ExtAudioFilePropertyID,
    _ ioPropertyDataSize: UnsafeMutablePointer,
    _ outPropertyData: UnsafeMutableRawPointer
) -> OSStatus
```

## Parameters 

`inExtAudioFile`  

The extended audio file object to get a property value from.

`inPropertyID`  

The property whose value you want.

`ioPropertyDataSize`  

On input, the size of the memory pointed to by the `outPropertyData` parameter. On output, the size of the property value.

`outPropertyData`  

On output, the property value you wanted to get.

## Return Value

A result code.

## Discussion

Some Core Audio property values are C types and others are Core Foundation objects.

If you call this function to retrieve a value that is a Core Foundation object, then this function—despite the use of “Get” in its name—duplicates the object. You are responsible for releasing the object, as described in The Create Rule in Memory Management Programming Guide for Core Foundation.

## See Also

### Configuring Properties for Extended Audio File Objects

func ExtAudioFileGetPropertyInfo(ExtAudioFileRef, ExtAudioFilePropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets information about an extended audio file object property.

func ExtAudioFileSetProperty(ExtAudioFileRef, ExtAudioFilePropertyID, UInt32, UnsafeRawPointer) -> OSStatus

Sets a property value for an extended audio file object.

