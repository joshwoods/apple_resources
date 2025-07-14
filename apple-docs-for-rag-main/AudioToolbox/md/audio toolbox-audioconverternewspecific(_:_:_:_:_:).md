

- Audio Toolbox
-  AudioConverterNewSpecific(\_:\_:\_:\_:\_:) 

Function

# AudioConverterNewSpecific(\_:\_:\_:\_:\_:)

Creates a new audio converter object using a specified codec.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func AudioConverterNewSpecific(
    _ inSourceFormat: UnsafePointer,
    _ inDestinationFormat: UnsafePointer,
    _ inNumberClassDescriptions: UInt32,
    _ inClassDescriptions: UnsafePointer,
    _ outAudioConverter: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inSourceFormat`  

The format of the source audio to be converted.

`inDestinationFormat`  

The destination format to which the audio is to be converted.

`inNumberClassDescriptions`  

The number of class descriptions supplied in the `inClassDescriptions` parameter.

`inClassDescriptions`  

A list of `AudioClassDescription` objects that specify the codec to use.

`outAudioConverter`  

On return, a new audio converter object.

## Return Value

A result code.

## Discussion

This function is identical to AudioConverterNew(_:_:_:) function, except that your application may explicitly choose which codec to instantiate if there is more than one choice.

## See Also

### Managing Audio Converter Objects

func AudioConverterNew(UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioStreamBasicDescription>, UnsafeMutablePointer&lt;AudioConverterRef?>) -> OSStatus

Creates a new audio converter object based on specified audio formats.

func AudioConverterReset(AudioConverterRef) -> OSStatus

Resets an audio converter object, clearing and flushing its buffers.

func AudioConverterDispose(AudioConverterRef) -> OSStatus

Disposes of an audio converter object.

