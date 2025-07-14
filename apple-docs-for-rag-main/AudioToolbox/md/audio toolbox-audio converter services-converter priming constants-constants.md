

- Audio Toolbox
- Audio Converter Services
-  Converter Priming Constants 

API Collection

# Converter Priming Constants

Constants used with the kAudioConverterPrimeMethod property.

## Topics

### Constants

var kConverterPrimeMethod_Pre: UInt32

Prime with `leading` + `trailing` input frames.

var kConverterPrimeMethod_Normal: UInt32

Prime with `trailing` frames only, for zero latency. Leading frames are assumed to be silence.

var kConverterPrimeMethod_None: UInt32

Acts in “latency” mode. Leading and trailing frames are both assumed to be silence.

## See Also

### Constants

Audio Converter Properties

Audio converter properties, used with the AudioConverterGetPropertyInfo(_:_:_:_:), AudioConverterGetProperty(_:_:_:_:), and AudioConverterSetProperty(_:_:_:_:) functions.

Sample Rate Conversion Quality Identifiers

Specifiers for sample rate conversion quality, used for the kAudioConverterSampleRateConverterQuality property.

Sample Rate Conversion Complexity Identifiers

Specifiers for the sample rate conversion algorithm, used for the kAudioConverterSampleRateConverterComplexity property.

