

- Audio Toolbox
- Audio Converter Services
-  Sample Rate Conversion Complexity Identifiers 

API Collection

# Sample Rate Conversion Complexity Identifiers

Specifiers for the sample rate conversion algorithm, used for the kAudioConverterSampleRateConverterComplexity property.

## Topics

### Constants

var kAudioConverterSampleRateConverterComplexity_Linear: UInt32

Specifies linear interpolation for sample rate conversion. This provides the lowest quality and is, computationally, the least expensive option.

var kAudioConverterSampleRateConverterComplexity_Normal: UInt32

Specifies the normal-complexity sample rate conversion algorithm. This is the default value.

var kAudioConverterSampleRateConverterComplexity_Mastering: UInt32

Specifies a mastering-quality sample rate conversion algorithm. This provides the highest quality and is, computationally, the most expensive option.

var kAudioConverterSampleRateConverterComplexity_MinimumPhase: UInt32

## See Also

### Constants

Audio Converter Properties

Audio converter properties, used with the AudioConverterGetPropertyInfo(_:_:_:_:), AudioConverterGetProperty(_:_:_:_:), and AudioConverterSetProperty(_:_:_:_:) functions.

Converter Priming Constants

Constants used with the kAudioConverterPrimeMethod property.

Sample Rate Conversion Quality Identifiers

Specifiers for sample rate conversion quality, used for the kAudioConverterSampleRateConverterQuality property.

