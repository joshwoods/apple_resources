

- Audio Toolbox
-  AudioConverterGetProperty(\_:\_:\_:\_:) 

Function

# AudioConverterGetProperty(\_:\_:\_:\_:)

Gets an audio converter property value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.1+tvOS 9.0+visionOS 1.0+

``` source
func AudioConverterGetProperty(
    _ inAudioConverter: AudioConverterRef,
    _ inPropertyID: AudioConverterPropertyID,
    _ ioPropertyDataSize: UnsafeMutablePointer,
    _ outPropertyData: UnsafeMutableRawPointer
) -> OSStatus
```

## Parameters 

`inAudioConverter`  

The audio converter to get a property value from.

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

### Configuring Audio Converter Properties

func AudioConverterGetPropertyInfo(AudioConverterRef, AudioConverterPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets information about an audio converter property.

func AudioConverterSetProperty(AudioConverterRef, AudioConverterPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

Sets the value of an audio converter object property.

