

- Audio Toolbox
-  AudioCodecAppendInputData(\_:\_:\_:\_:\_:) 

Function

# AudioCodecAppendInputData(\_:\_:\_:\_:\_:)

Appends audio data to the codec’s input buffer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func AudioCodecAppendInputData(
    _ inCodec: AudioCodec,
    _ inInputData: UnsafeRawPointer,
    _ ioInputDataByteSize: UnsafeMutablePointer,
    _ ioNumberPackets: UnsafeMutablePointer,
    _ inPacketDescription: UnsafePointer?
) -> OSStatus
```

## Parameters 

`inCodec`  

An audio codec object. Because an audio codec object is a Component Manger component instance, you can use the Component Manager (for example, the functions FindNextComponent and OpenAComponent) to obtain an audio codec object.

`inInputData`  

The audio data to be sent to the codec. Indicate there is no more data to process by passing a buffer of `0`bytes.

`ioInputDataByteSize`  

On input, the size in bytes of the data pointed to by the `inInputData` parameter. On output, the number of bytes the codec actually appended to its input buffer.

`ioNumberPackets`  

On input, the number of elements in the `inPacketDescription` array. Pass `NULL` for this parameter if the input data has a constant number of frames per packet. On return, the number of packets actually processed by the codec.

`inPacketDescription`  

For audio data that has a variable number of frames per packet, an array of `AudioStreamPacketDescription` structures that describes the packet layout. Pass `NULL` for this parameter if the input data has a constant number of frames per packet.

## Return Value

Returns `NoErr` if successful. Returns `kAudioCodecStateError` if the codec has not been initialized. See `Result Codes` for other possible values.

## Discussion

A packet is the smallest, indivisible block of data for a given audio format. For linear PCM (pulse-code modulated) data, each packet contains exactly one frame, where a frame is a set of samples representing one sample for each channel. For compressed audio data formats, the number of frames in a packet depends on the encoding. For example, a packet of AAC represents 1024 frames of PCM. In some formats, the number of frames per packet varies. For such formats, you must include an array of `AudioStreamPacketDescription` structures that describes the packet layout.

Input data can be fed into an encoder and some decoders in blocks of any size (even byte by byte). However, if the encoded format of the input data fed to a decoder has a variable number of frames per packet, the data must be provided in multiples of whole packets. A codec’s properties provide information about allowable types of input and output, minimum and maximum buffer sizes, and so forth. Use the AudioCodecGetProperty(_:_:_:_:) function to read a codec’s properties. The properties are described in Global Codec Properties and Instance Codec Properties.

The combination of the AudioCodecAppendInputData(_:_:_:_:_:) and AudioCodecProduceOutputPackets(_:_:_:_:_:_:) functions implement a “push-pull” model of data handling. First, the input data is pushed into the codec, then the resulting output data is pulled out of that same codec.

## See Also

### Related Documentation

func AudioCodecInitialize(AudioCodec, UnsafePointer&lt;AudioStreamBasicDescription>?, UnsafePointer&lt;AudioStreamBasicDescription>?, UnsafeRawPointer?, UInt32) -> OSStatus

Sets up the specified codec to perform a data format translation.

func AudioCodecGetProperty(AudioCodec, AudioCodecPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Retrieves the value of a codec property.

### Accessing the Data

func AudioCodecProduceOutputPackets(AudioCodec, UnsafeMutableRawPointer, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Retrieves output data from a codec.

