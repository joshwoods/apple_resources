

- Audio Toolbox
-  AudioConverterSetProperty(\_:\_:\_:\_:) 

Function

# AudioConverterSetProperty(\_:\_:\_:\_:)

Sets the value of an audio converter object property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.1+tvOS 9.0+visionOS 1.0+

``` source
func AudioConverterSetProperty(
    _ inAudioConverter: AudioConverterRef,
    _ inPropertyID: AudioConverterPropertyID,
    _ inPropertyDataSize: UInt32,
    _ inPropertyData: UnsafeRawPointer
) -> OSStatus
```

## Parameters 

`inAudioConverter`  

The audio converter to set a property value on.

`inPropertyID`  

The property whose value you want to set.

`inPropertyDataSize`  

The size, in bytes, of the property value.

`inPropertyData`  

The value you want to apply to the specified property.

## Return Value

A result code.

## Discussion

You can employ the property mechanism, for example, to split a monaural input to both channels of a stereo output. You would do this as follows:

```
```

## See Also

### Configuring Audio Converter Properties

func AudioConverterGetProperty(AudioConverterRef, AudioConverterPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Gets an audio converter property value.

func AudioConverterGetPropertyInfo(AudioConverterRef, AudioConverterPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets information about an audio converter property.

