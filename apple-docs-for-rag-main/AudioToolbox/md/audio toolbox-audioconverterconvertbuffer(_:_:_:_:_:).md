

- Audio Toolbox
-  AudioConverterConvertBuffer(\_:\_:\_:\_:\_:) 

Function

# AudioConverterConvertBuffer(\_:\_:\_:\_:\_:)

Converts audio data from one linear PCM format to another.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.1+tvOS 9.0+visionOS 1.0+

``` source
func AudioConverterConvertBuffer(
    _ inAudioConverter: AudioConverterRef,
    _ inInputDataSize: UInt32,
    _ inInputData: UnsafeRawPointer,
    _ ioOutputDataSize: UnsafeMutablePointer,
    _ outOutputData: UnsafeMutableRawPointer
) -> OSStatus
```

## Parameters 

`inAudioConverter`  

The audio converter to use for format conversion.

`inInputDataSize`  

The size, in bytes, of the audio data input buffer.

`inInputData`  

The audio data to convert.

`ioOutputDataSize`  

On input, the size, in bytes, of the buffer available for the converted data. On output, the number of bytes written to the output buffer (pointed to by the `outOutputData` parameter).

`outOutputData`  

On output, the converted audio data.

## Return Value

A result code.

## Discussion

This function is for the special case of converting from one linear PCM format to another. This function cannot perform sample rate conversions and cannot be used for conversion to or from most compressed formats. To perform these types of conversion, use AudioConverterFillComplexBuffer(_:_:_:_:_:_:) instead.

## See Also

### Performing Conversions

Encoding and decoding audio

Convert audio formats to efficiently manage data and quality.

func AudioConverterFillComplexBuffer(AudioConverterRef, AudioConverterComplexInputDataProc, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioBufferList>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?) -> OSStatus

Converts audio data supplied by a callback function, supporting non-interleaved and packetized formats.

func AudioConverterConvertComplexBuffer(AudioConverterRef, UInt32, UnsafePointer&lt;AudioBufferList>, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

Converts audio data from one linear PCM format to another, where both use the same sample rate.

