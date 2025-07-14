

- Audio Toolbox
-  AudioConverterGetPropertyInfo(\_:\_:\_:\_:) 

Function

# AudioConverterGetPropertyInfo(\_:\_:\_:\_:)

Gets information about an audio converter property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.1+tvOS 9.0+visionOS 1.0+

``` source
func AudioConverterGetPropertyInfo(
    _ inAudioConverter: AudioConverterRef,
    _ inPropertyID: AudioConverterPropertyID,
    _ outSize: UnsafeMutablePointer?,
    _ outWritable: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`inAudioConverter`  

The audio converter to get property information from.

`inPropertyID`  

The property you want information about.

`outSize`  

On output, the size of the property value in bytes. Can be `NULL` on output.

`outWritable`  

On output, a Boolean value indicating whether the property value is writable (`true`) or not (`false`). Can be `NULL` on output.

## Return Value

A result code.

## See Also

### Configuring Audio Converter Properties

func AudioConverterGetProperty(AudioConverterRef, AudioConverterPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Gets an audio converter property value.

func AudioConverterSetProperty(AudioConverterRef, AudioConverterPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

Sets the value of an audio converter object property.

