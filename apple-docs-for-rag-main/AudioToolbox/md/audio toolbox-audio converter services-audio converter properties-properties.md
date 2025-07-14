

- Audio Toolbox
- Audio Converter Services
-  Audio Converter Properties 

API Collection

# Audio Converter Properties

Audio converter properties, used with the AudioConverterGetPropertyInfo(_:_:_:_:), AudioConverterGetProperty(_:_:_:_:), and AudioConverterSetProperty(_:_:_:_:) functions.

## Topics

### Constants

var kAudioConverterPropertyMinimumInputBufferSize: AudioConverterPropertyID

A `UInt32` value that indicates the size, in bytes, of the smallest buffer of input data that can be supplied via the audio converter input callback or as the input to the AudioConverterConvertBuffer(_:_:_:_:_:) function.

var kAudioConverterPropertyMinimumOutputBufferSize: AudioConverterPropertyID

A `UInt32` value that indicates the size, in bytes, of the smallest buffer of output data that can be supplied to AudioConverterFillComplexBuffer or as the output to AudioConverterConvertBuffer

var kAudioConverterPropertyMaximumInputBufferSize: AudioConverterPropertyID

Deprecated. The audio converter input callback may be passed any number of packets of data. If fewer are packets are returned than required, then the input proc is called again. If more packets are passed than required, they remain in the client’s buffer and are consumed as needed.

var kAudioConverterPropertyMaximumInputPacketSize: AudioConverterPropertyID

A `UInt32` value that indicates the size, in bytes, of the largest single packet of data in the input format. This is mostly useful for variable bit rate compressed data (decoders).

var kAudioConverterPropertyMaximumOutputPacketSize: AudioConverterPropertyID

A `UInt32` value that indicates the size, in bytes, of the largest single packet of data in the output format. This is mostly useful for variable bit rate compressed data (encoders).

var kAudioConverterPropertyCalculateInputBufferSize: AudioConverterPropertyID

A `UInt32` value that on input holds a size, in bytes, that is desired for the output data. On output, it holds the size, in bytes, of the input buffer required to generate that much output data. Note that some converters cannot do this calculation.

var kAudioConverterPropertyCalculateOutputBufferSize: AudioConverterPropertyID

A `UInt32` value that on input holds a size, in bytes, that is desired for the input data. On output, it holds the size, in bytes, of the output buffer required to hold the output data to be generated. Some converters cannot do this calculation.

var kAudioConverterPropertyInputCodecParameters: AudioConverterPropertyID

The value of this property varies from format to format and is considered private to the format. It is treated as a buffer of untyped data.

var kAudioConverterPropertyOutputCodecParameters: AudioConverterPropertyID

The value of this property varies from format to format and is considered private to the format. It is treated as a buffer of untyped data.

var kAudioConverterSampleRateConverterAlgorithm: AudioConverterPropertyID

A value that indicates the sample rate conversion algorithm.

var kAudioConverterSampleRateConverterComplexity: AudioConverterPropertyID

The sample rate conversion algorithm.

var kAudioConverterSampleRateConverterQuality: AudioConverterPropertyID

The rendering quality of the sample rate converter.

var kAudioConverterSampleRateConverterInitialPhase: AudioConverterPropertyID

A `Float64` value equal to `0.0`.

var kAudioConverterCodecQuality: AudioConverterPropertyID

The rendering quality of a codec. A `UInt32` value.

var kAudioConverterPrimeMethod: AudioConverterPropertyID

The priming method, usually for sample-rate conversion.

var kAudioConverterPrimeInfo: AudioConverterPropertyID

An AudioConverterPrimeInfo structure.

var kAudioConverterChannelMap: AudioConverterPropertyID

An array of `SInt32` values that specify an input-to-output channel mapping.

var kAudioConverterDecompressionMagicCookie: AudioConverterPropertyID

A `void*` value that points to memory set up by the caller. This property is required by some audio data formats in order to decompress the input data.

var kAudioConverterCompressionMagicCookie: AudioConverterPropertyID

A `void*` value that points to memory set up by the caller. This property is returned by the converter so that your application may store it along with the output data. This property can then be passed back to the converter for decompression at a later time.

var kAudioConverterEncodeBitRate: AudioConverterPropertyID

A `UInt32` value containing the number of bits per second to aim for when encoding data. Some decoders also allow you to query this property to discover the bit rate.

var kAudioConverterEncodeAdjustableSampleRate: AudioConverterPropertyID

A `Float64` value that specifies an output sample rate.

var kAudioConverterInputChannelLayout: AudioConverterPropertyID

An `AudioChannelLayout` structure that specifies an audio converter’s input channel layout.

var kAudioConverterOutputChannelLayout: AudioConverterPropertyID

An `AudioChannelLayout` structure that specifies an audio converter’s output channel layout.

var kAudioConverterApplicableEncodeBitRates: AudioConverterPropertyID

An array of `AudioValueRange` structures that describes applicable bit rates based on current settings.

var kAudioConverterAvailableEncodeBitRates: AudioConverterPropertyID

An array of `AudioValueRange` structures that describes the available bit rates based on the input format. You can determine the available bit rates using Audio Format Services.

var kAudioConverterApplicableEncodeSampleRates: AudioConverterPropertyID

An array of `AudioValueRange` structures that describes applicable sample rates based on current settings.

var kAudioConverterAvailableEncodeSampleRates: AudioConverterPropertyID

An array of `AudioValueRange` structures that describes the available sample rates based on the input format. You can determine the available sample rates using Audio Format Services.

var kAudioConverterAvailableEncodeChannelLayoutTags: AudioConverterPropertyID

An array of `AudioChannelLayoutTag` values for the format and number of channels specified in the encoder’s input format.

var kAudioConverterCurrentOutputStreamDescription: AudioConverterPropertyID

The current, completely specified output `AudioStreamBasicDescription` structure.

var kAudioConverterCurrentInputStreamDescription: AudioConverterPropertyID

The current, completely specified input `AudioStreamBasicDescription` structure.

var kAudioConverterPropertySettings: AudioConverterPropertyID

An array (of type `CFArray`) of property settings for converters.

var kAudioConverterPropertyBitDepthHint: AudioConverterPropertyID

A `UInt32` value that designates the source bit depth to preserve.

var kAudioConverterPropertyFormatList: AudioConverterPropertyID

An array of `AudioFormatListItem` structures that describes the set of data formats produced by the encoder end of an audio converter.

var kAudioConverterPropertyCanResumeFromInterruption: AudioConverterPropertyID

Indicates whether the underlying codec supports resumption of processing following an audio interruption. A read-only `UInt32` value.

## See Also

### Constants

Converter Priming Constants

Constants used with the kAudioConverterPrimeMethod property.

Sample Rate Conversion Quality Identifiers

Specifiers for sample rate conversion quality, used for the kAudioConverterSampleRateConverterQuality property.

Sample Rate Conversion Complexity Identifiers

Specifiers for the sample rate conversion algorithm, used for the kAudioConverterSampleRateConverterComplexity property.

