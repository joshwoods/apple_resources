

- Audio Toolbox
-  AudioConverterDispose(\_:) 

Function

# AudioConverterDispose(\_:)

Disposes of an audio converter object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.1+tvOS 9.0+visionOS 1.0+

``` source
func AudioConverterDispose(_ inAudioConverter: AudioConverterRef) -> OSStatus
```

## Parameters 

`inAudioConverter`  

The audio converter object to dispose of.

## Return Value

A result code.

## Discussion

## See Also

### Managing Audio Converter Objects

func AudioConverterNew(UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioStreamBasicDescription>, UnsafeMutablePointer&lt;AudioConverterRef?>) -> OSStatus

Creates a new audio converter object based on specified audio formats.

func AudioConverterNewSpecific(UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32, UnsafePointer&lt;AudioClassDescription>, UnsafeMutablePointer&lt;AudioConverterRef?>) -> OSStatus

Creates a new audio converter object using a specified codec.

func AudioConverterReset(AudioConverterRef) -> OSStatus

Resets an audio converter object, clearing and flushing its buffers.

