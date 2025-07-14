

- Audio Toolbox
-  kAudioConverterErr_HardwareInUse 

Global Variable

# kAudioConverterErr_HardwareInUse

Returned from the AudioConverterFillComplexBuffer(_:_:_:_:_:_:) function if the underlying hardware codec has become unavailable, probably due to an audio interruption.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
var kAudioConverterErr_HardwareInUse: OSStatus { get }
```

## Discussion

On receiving this error, your application must stop calling `AudioConverterFillComplexBuffer`. You can check the value of the kAudioConverterPropertyCanResumeFromInterruption property to determine if the converter you are using can resume processing after an interruption. If so, then wait for an interruption-ended call from Audio Session Services, reactivate the audio session, and finally resume using the codec.

If the converter cannot resume processing after an interruption, then on interruption you must abandon the conversion, re-instantiate the converter, and perform the conversion again.

## See Also

### Result Codes

var kAudioConverterErr_FormatNotSupported: OSStatus

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

var kAudioConverterErr_NoHardwarePermission: OSStatus

Returned from the AudioConverterNew(_:_:_:) function if the new converter would use a hardware codec which the application does not have permission to use.

