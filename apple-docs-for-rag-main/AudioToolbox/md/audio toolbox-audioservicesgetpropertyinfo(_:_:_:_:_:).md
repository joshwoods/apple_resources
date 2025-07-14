

- Audio Toolbox
-  AudioServicesGetPropertyInfo(\_:\_:\_:\_:\_:) 

Function

# AudioServicesGetPropertyInfo(\_:\_:\_:\_:\_:)

Gets information about a System Sound Services property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioServicesGetPropertyInfo(
    _ inPropertyID: AudioServicesPropertyID,
    _ inSpecifierSize: UInt32,
    _ inSpecifier: UnsafeRawPointer?,
    _ outPropertyDataSize: UnsafeMutablePointer?,
    _ outWritable: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`inPropertyID`  

The property you want information about.

`inSpecifierSize`  

The size of the buffer pointed to by the `inSpecifier` parameter. Pass `0` if no specifier buffer is required.

`inSpecifier`  

A pointer to a specifier buffer, if such a buffer is required by the property about which you want information. Pass `NULL` if no specifier is required.

`outPropertyDataSize`  

On output, the size, in bytes, of the property value. To get the property value, you need a buffer of at least this size.

`outWritable`  

On output, `true` if the property is writable, or `false` if the property is read only.

## Return Value

A result code.

## Discussion

System Sound Services properties are listed and described in System Sound Services Property Identifiers.

## See Also

### Managing System Sound Services Properties

func AudioServicesGetProperty(AudioServicesPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer?) -> OSStatus

Gets a specified System Sound Services property value.

func AudioServicesSetProperty(AudioServicesPropertyID, UInt32, UnsafeRawPointer?, UInt32, UnsafeRawPointer) -> OSStatus

Sets the value for a specified System Sound Services property.

typealias AudioServicesPropertyID

The data type for a system sound property identifier.

System Sound Services Property Identifiers

Property identifiers used when playing alerts with System Sound Services.

Audio Hardware Services Properties

Property identifiers that apply to HAL audio objects only when accessed via the Audio Hardware Services.

