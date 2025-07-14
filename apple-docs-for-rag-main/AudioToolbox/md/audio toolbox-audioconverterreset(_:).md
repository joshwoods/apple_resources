

- Audio Toolbox
-  AudioConverterReset(\_:) 

Function

# AudioConverterReset(\_:)

Resets an audio converter object, clearing and flushing its buffers.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.1+tvOS 9.0+visionOS 1.0+

``` source
func AudioConverterReset(_ inAudioConverter: AudioConverterRef) -> OSStatus
```

## Parameters 

`inAudioConverter`  

The audio converter object to reset.

## Return Value

A result code.

## Discussion

Call this function after a discontinuity in the source audio stream being provided to the converter.

## See Also

### Managing Audio Converter Objects

func AudioConverterNew(UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioStreamBasicDescription>, UnsafeMutablePointer&lt;AudioConverterRef?>) -> OSStatus

Creates a new audio converter object based on specified audio formats.

func AudioConverterNewSpecific(UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32, UnsafePointer&lt;AudioClassDescription>, UnsafeMutablePointer&lt;AudioConverterRef?>) -> OSStatus

Creates a new audio converter object using a specified codec.

func AudioConverterDispose(AudioConverterRef) -> OSStatus

Disposes of an audio converter object.

