

- Audio Toolbox
- Audio Converter Services
-  Audio Converter Errors 

API Collection

# Audio Converter Errors

## Topics

### Constants

var kAudioConverterErr_BadPropertySizeError: OSStatus

var kAudioConverterErr_FormatNotSupported: OSStatus

var kAudioConverterErr_HardwareInUse: OSStatus

Returned from the AudioConverterFillComplexBuffer(_:_:_:_:_:_:) function if the underlying hardware codec has become unavailable, probably due to an audio interruption.

var kAudioConverterErr_InputSampleRateOutOfRange: OSStatus

var kAudioConverterErr_InvalidInputSize: OSStatus

var kAudioConverterErr_InvalidOutputSize: OSStatus

The byte size is not an integer multiple of the frame size.

var kAudioConverterErr_NoHardwarePermission: OSStatus

Returned from the AudioConverterNew(_:_:_:) function if the new converter would use a hardware codec which the application does not have permission to use.

var kAudioConverterErr_OperationNotSupported: OSStatus

var kAudioConverterErr_OutputSampleRateOutOfRange: OSStatus

var kAudioConverterErr_PropertyNotSupported: OSStatus

var kAudioConverterErr_RequiresPacketDescriptionsError: OSStatus

var kAudioConverterErr_UnspecifiedError: OSStatus

## See Also

### Enumerations

Converter Audio Unit Properties

Properties for the Apple AUConverter audio unit.

Converter Audio Unit Subtypes

Audio data format converter audio unit subtypes for audio units provided by Apple.

Audio Converter Dithering Algorithms

Audio Converter Properties (macOS)

