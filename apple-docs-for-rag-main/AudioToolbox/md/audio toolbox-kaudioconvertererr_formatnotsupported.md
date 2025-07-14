

- Audio Toolbox
-  kAudioConverterErr_FormatNotSupported 

Global Variable

# kAudioConverterErr_FormatNotSupported

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioConverterErr_FormatNotSupported: OSStatus { get }
```

## See Also

### Result Codes

var kAudioConverterErr_OperationNotSupported: OSStatus

var kAudioConverterErr_PropertyNotSupported: OSStatus

var kAudioConverterErr_InvalidInputSize: OSStatus

var kAudioConverterErr_InvalidOutputSize: OSStatus

The byte size is not an integer multiple of the frame size.

var kAudioConverterErr_UnspecifiedError: OSStatus

var kAudioConverterErr_BadPropertySizeError: OSStatus

var kAudioConverterErr_RequiresPacketDescriptionsError: OSStatus

var kAudioConverterErr_InputSampleRateOutOfRange: OSStatus

var kAudioConverterErr_OutputSampleRateOutOfRange: OSStatus

var kAudioConverterErr_HardwareInUse: OSStatus

Returned from the AudioConverterFillComplexBuffer(_:_:_:_:_:_:) function if the underlying hardware codec has become unavailable, probably due to an audio interruption.

var kAudioConverterErr_NoHardwarePermission: OSStatus

Returned from the AudioConverterNew(_:_:_:) function if the new converter would use a hardware codec which the application does not have permission to use.

