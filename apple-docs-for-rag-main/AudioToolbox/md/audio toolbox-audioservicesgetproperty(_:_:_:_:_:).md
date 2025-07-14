

- Audio Toolbox
-  AudioServicesGetProperty(\_:\_:\_:\_:\_:) 

Function

# AudioServicesGetProperty(\_:\_:\_:\_:\_:)

Gets a specified System Sound Services property value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioServicesGetProperty(
    _ inPropertyID: AudioServicesPropertyID,
    _ inSpecifierSize: UInt32,
    _ inSpecifier: UnsafeRawPointer?,
    _ ioPropertyDataSize: UnsafeMutablePointer,
    _ outPropertyData: UnsafeMutableRawPointer?
) -> OSStatus
```

## Parameters 

`inPropertyID`  

The property whose value you want.

`inSpecifierSize`  

The size of the buffer pointed to by the `inSpecifier` parameter. Pass `0` if no specifier buffer is required.

`inSpecifier`  

A pointer to a specifier buffer, if such a buffer is required by the property about which you want information. Pass `NULL` if no specifier is required.

`ioPropertyDataSize`  

On input, the size, in bytes, of the buffer pointed to by the `outPropertyData` parameter. Call the AudioServicesGetPropertyInfo(_:_:_:_:_:) function to find out the size required for this buffer. On output, the number of bytes written to the buffer.

`outPropertyData`  

On output, the property value.

## Return Value

A result code.

## Discussion

System Sound Services properties are listed and described in System Sound Services Property Identifiers.

### Special Considerations

Some Core Audio property values are C types and others are Core Foundation objects.

If you call this function to retrieve a value that is a Core Foundation object, then this function—despite the use of “Get” in its name—duplicates the object. You are responsible for releasing the object, as described in The Create Rule in Memory Management Programming Guide for Core Foundation.

## See Also

### Managing System Sound Services Properties

func AudioServicesGetPropertyInfo(AudioServicesPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets information about a System Sound Services property.

func AudioServicesSetProperty(AudioServicesPropertyID, UInt32, UnsafeRawPointer?, UInt32, UnsafeRawPointer) -> OSStatus

Sets the value for a specified System Sound Services property.

typealias AudioServicesPropertyID

The data type for a system sound property identifier.

System Sound Services Property Identifiers

Property identifiers used when playing alerts with System Sound Services.

Audio Hardware Services Properties

Property identifiers that apply to HAL audio objects only when accessed via the Audio Hardware Services.

