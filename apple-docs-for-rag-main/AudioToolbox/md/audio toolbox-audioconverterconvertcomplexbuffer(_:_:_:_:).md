

- Audio Toolbox
-  AudioConverterConvertComplexBuffer(\_:\_:\_:\_:) 

Function

# AudioConverterConvertComplexBuffer(\_:\_:\_:\_:)

Converts audio data from one linear PCM format to another, where both use the same sample rate.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func AudioConverterConvertComplexBuffer(
    _ inAudioConverter: AudioConverterRef,
    _ inNumberPCMFrames: UInt32,
    _ inInputData: UnsafePointer,
    _ outOutputData: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inAudioConverter`  

The audio converter to use for the format conversion.

`inNumberPCMFrames`  

The number of linear PCM frames to convert.

`inInputData`  

The source audio buffer list.

`outOutputData`  

The destination audio buffer list.

## Return Value

A result code.

## Discussion

This function is appropriate for linear PCM-to-linear PCM audio data format conversion where there is no sample rate conversion.

Important

This function fails for conversions where there is a variation between the input and output data buffer sizes. This includes sample rate conversions and conversions involving most compressed formats. In these cases, instead use the AudioConverterFillComplexBuffer(_:_:_:_:_:_:) function.

## See Also

### Performing Conversions

Encoding and decoding audio

Convert audio formats to efficiently manage data and quality.

func AudioConverterConvertBuffer(AudioConverterRef, UInt32, UnsafeRawPointer, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Converts audio data from one linear PCM format to another.

func AudioConverterFillComplexBuffer(AudioConverterRef, AudioConverterComplexInputDataProc, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioBufferList>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?) -> OSStatus

Converts audio data supplied by a callback function, supporting non-interleaved and packetized formats.

