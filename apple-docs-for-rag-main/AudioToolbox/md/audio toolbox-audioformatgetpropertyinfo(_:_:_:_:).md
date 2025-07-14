

- Audio Toolbox
-  AudioFormatGetPropertyInfo(\_:\_:\_:\_:) 

Function

# AudioFormatGetPropertyInfo(\_:\_:\_:\_:)

Gets information about an audio format property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+

``` source
func AudioFormatGetPropertyInfo(
    _ inPropertyID: AudioFormatPropertyID,
    _ inSpecifierSize: UInt32,
    _ inSpecifier: UnsafeRawPointer?,
    _ outPropertyDataSize: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inPropertyID`  

An `AudioFormatPropertyID` constant.

`inSpecifierSize`  

The size of the specifier data.

`inSpecifier`  

A buffer of data used as an input argument for querying some of the properties.

`outPropertyDataSize`  

The the size in bytes of the current value of the property. To get the property value, you need a buffer of this size.

## Return Value

A result code. Returns `noErr` if successful.

## See Also

### Audio Format Services Functions

func AudioFormatGetProperty(AudioFormatPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutableRawPointer?) -> OSStatus

Gets the value of an audio format property.

