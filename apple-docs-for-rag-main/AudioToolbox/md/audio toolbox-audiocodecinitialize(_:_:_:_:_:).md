

- Audio Toolbox
-  AudioCodecInitialize(\_:\_:\_:\_:\_:) 

Function

# AudioCodecInitialize(\_:\_:\_:\_:\_:)

Sets up the specified codec to perform a data format translation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func AudioCodecInitialize(
    _ inCodec: AudioCodec,
    _ inInputFormat: UnsafePointer?,
    _ inOutputFormat: UnsafePointer?,
    _ inMagicCookie: UnsafeRawPointer?,
    _ inMagicCookieByteSize: UInt32
) -> OSStatus
```

## Parameters 

`inCodec`  

An audio codec object. Because an audio codec object is a Component Manager component instance, you can use the Component Manager (for example, the functions FindNextComponent and OpenAComponent) to obtain an audio codec object.

`inInputFormat`  

A structure that describes the format of the input data. See Core Audio Data Types for a description of this structure and the values of constants that can be used in this structure. If the input data has a variable number of frames per packet, this structure is supplemented with the `AudioStreamPacketDescription` structure passed in the `inPacketDescription` parameter of the AudioCodecAppendInputData(_:_:_:_:_:) function.

`inOutputFormat`  

A structure that describes the format desired for the output data.

`inMagicCookie`  

Magic cookie data, if required for the input format.

`inMagicCookieByteSize`  

Size in bytes of the magic cookie data, if any.

## Return Value

Returns `NoErr` if successful. Returns `kAudioCodecUnsupportedFormatError` if the codec cannot handle the specified data translation. See `Result Codes` for other possible values.

## Discussion

This function allocates any buffers needed, sets the input and output formats, and puts the codec into the initialized state. The codec has to be in the initialized state for the AudioCodecAppendInputData(_:_:_:_:_:) and AudioCodecProduceOutputPackets(_:_:_:_:_:_:) functions to work. While in this state, the format information for the translation cannot be changed; you must call the AudioCodecUninitialize(_:) function before making any changes. A codec’s properties provide information about allowable types of input and output, magic cookies, and so forth. Use the AudioCodecGetProperty(_:_:_:_:) function to read a codec’s properties. The properties are described in Global Codec Properties and Instance Codec Properties.

If any argument is `NULL`, any values previously set for that argument are used. For example, if you are using the same codec repeatedly with the same input and output formats, you only need to enter the formats the first time you initialize the codec. After that, you can uninitialize, change property values as necessary, and then call this function again with `NULL` in the `inInputFormat` and `inOutputFormat` parameters before processing the next set of data.

## See Also

### Related Documentation

func AudioCodecProduceOutputPackets(AudioCodec, UnsafeMutableRawPointer, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Retrieves output data from a codec.

func AudioCodecAppendInputData(AudioCodec, UnsafeRawPointer, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;UInt32>, UnsafePointer&lt;AudioStreamPacketDescription>?) -> OSStatus

Appends audio data to the codec’s input buffer.

func AudioCodecGetProperty(AudioCodec, AudioCodecPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Retrieves the value of a codec property.

### Initializing an Audio Codec

func AudioCodecReset(AudioCodec) -> OSStatus

Flushes all the audio data in the codec and clears the input buffer.

func AudioCodecUninitialize(AudioCodec) -> OSStatus

Moves the codec from the initialized state back to the uninitialized state.

