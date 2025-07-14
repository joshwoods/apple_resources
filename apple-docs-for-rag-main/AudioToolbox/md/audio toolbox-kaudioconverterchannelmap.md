

- Audio Toolbox
-  kAudioConverterChannelMap 

Global Variable

# kAudioConverterChannelMap

An array of `SInt32` values that specify an input-to-output channel mapping.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioConverterChannelMap: AudioConverterPropertyID { get }
```

## Discussion

The size of the array is the number of output channels. Each element specifies, using a 0-based index, which input channel’s data is routed to that output channel. A value of `-1` indicates that no input channel is to be routed to that output channel.

The default behavior is as follows. Given that `In` = the number of input channels and `Out` = the number of output channels. When `In` \> `Out`, the first `Out` inputs are routed to the first `Out` outputs, and the remaining inputs are discarded. When `Out` \> `In`, the first `In` inputs are routed to the first `Out` outputs, and the remaining outputs are zeroed.

## See Also

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

