

- Audio Toolbox
-  AudioServicesSetProperty(\_:\_:\_:\_:\_:) 

Function

# AudioServicesSetProperty(\_:\_:\_:\_:\_:)

Sets the value for a specified System Sound Services property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioServicesSetProperty(
    _ inPropertyID: AudioServicesPropertyID,
    _ inSpecifierSize: UInt32,
    _ inSpecifier: UnsafeRawPointer?,
    _ inPropertyDataSize: UInt32,
    _ inPropertyData: UnsafeRawPointer
) -> OSStatus
```

## Parameters 

`inPropertyID`  

The property whose value you want to set.

`inSpecifierSize`  

The size of the buffer pointed to by the `inSpecifier` parameter. Pass `0` if no specifier buffer is required.

`inSpecifier`  

A pointer to a specifier buffer, if such a buffer is required by the property about which you want information. Pass `NULL` if no specifier is required.

`inPropertyDataSize`  

The size, in bytes, of the buffer pointed to by the `inPropertyData` parameter.

`inPropertyData`  

The property value you want to set.

## Return Value

A result code.

## Discussion

System Sound Services properties are listed and described in System Sound Services Property Identifiers.

## See Also

### Managing System Sound Services Properties

func AudioServicesGetPropertyInfo(AudioServicesPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets information about a System Sound Services property.

func AudioServicesGetProperty(AudioServicesPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer?) -> OSStatus

Gets a specified System Sound Services property value.

typealias AudioServicesPropertyID

The data type for a system sound property identifier.

System Sound Services Property Identifiers

Property identifiers used when playing alerts with System Sound Services.

Audio Hardware Services Properties

Property identifiers that apply to HAL audio objects only when accessed via the Audio Hardware Services.

