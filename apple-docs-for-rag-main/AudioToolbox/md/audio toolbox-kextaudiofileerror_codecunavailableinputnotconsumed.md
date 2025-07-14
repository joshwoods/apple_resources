

- Audio Toolbox
-  kExtAudioFileError_CodecUnavailableInputNotConsumed 

Global Variable

# kExtAudioFileError_CodecUnavailableInputNotConsumed

The ExtAudioFileWrite(_:_:_:) function was interrupted and the last buffer that you provided was *not* successfully written to disk.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
var kExtAudioFileError_CodecUnavailableInputNotConsumed: OSStatus { get }
```

## Discussion

For additional information, refer to Audio Guidelines By App Type in Audio Session Programming Guide.

## See Also

### Result Codes

var kExtAudioFileError_CodecUnavailableInputConsumed: OSStatus

The ExtAudioFileWrite(_:_:_:) function was interrupted and the last buffer that you provided was successfully written to disk.

var kExtAudioFileError_InvalidProperty: OSStatus

var kExtAudioFileError_InvalidPropertySize: OSStatus

var kExtAudioFileError_NonPCMClientFormat: OSStatus

var kExtAudioFileError_InvalidChannelMap: OSStatus

The number of channels does not match the specified format.

var kExtAudioFileError_InvalidOperationOrder: OSStatus

var kExtAudioFileError_InvalidDataFormat: OSStatus

var kExtAudioFileError_MaxPacketSizeUnknown: OSStatus

var kExtAudioFileError_InvalidSeek: OSStatus

An attempt to write, or an offset, is out of bounds.

var kExtAudioFileError_AsyncWriteTooLarge: OSStatus

var kExtAudioFileError_AsyncWriteBufferOverflow: OSStatus

An asynchronous write operation could not be completed in time.

