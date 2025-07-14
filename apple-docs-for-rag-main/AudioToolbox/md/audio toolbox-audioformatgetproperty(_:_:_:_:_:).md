

- Audio Toolbox
-  AudioFormatGetProperty(\_:\_:\_:\_:\_:) 

Function

# AudioFormatGetProperty(\_:\_:\_:\_:\_:)

Gets the value of an audio format property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+

``` source
func AudioFormatGetProperty(
    _ inPropertyID: AudioFormatPropertyID,
    _ inSpecifierSize: UInt32,
    _ inSpecifier: UnsafeRawPointer?,
    _ ioPropertyDataSize: UnsafeMutablePointer?,
    _ outPropertyData: UnsafeMutableRawPointer?
) -> OSStatus
```

## Parameters 

`inPropertyID`  

An AudioFormatPropertyID constant. For a list of these constants, see Audio Format Property Identifiers.

`inSpecifierSize`  

The size of the specifier data.

`inSpecifier`  

A buffer of data used as an input argument for querying some of the properties.

`ioPropertyDataSize`  

On input, the size of the `outPropertyData` buffer. On output, the number of bytes written to the buffer.

`outPropertyData`  

The buffer to write the property data to. If the `outPropertyData` parameter is `NULL` and `ioPropertyDataSize` is not `NULL`, the amount that would have been written is reported.

## Return Value

A result code. Returns `noErr` if successful.

## Discussion

Some Core Audio property values are C types and others are Core Foundation objects.

If you call this function to retrieve a value that is a Core Foundation object, then this function—despite the use of “Get” in its name—duplicates the object. You are responsible for releasing the object, as described in The Create Rule in Memory Management Programming Guide for Core Foundation.

## See Also

### Audio Format Services Functions

func AudioFormatGetPropertyInfo(AudioFormatPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets information about an audio format property.

