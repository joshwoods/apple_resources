

- Audio Toolbox
-  kExtAudioFileError_AsyncWriteTooLarge 

Global Variable

# kExtAudioFileError_AsyncWriteTooLarge

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kExtAudioFileError_AsyncWriteTooLarge: OSStatus { get }
```

## See Also

### Result Codes

var kExtAudioFileError_CodecUnavailableInputConsumed: OSStatus

The ExtAudioFileWrite(_:_:_:) function was interrupted and the last buffer that you provided was successfully written to disk.

var kExtAudioFileError_CodecUnavailableInputNotConsumed: OSStatus

The ExtAudioFileWrite(_:_:_:) function was interrupted and the last buffer that you provided was *not* successfully written to disk.

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

var kExtAudioFileError_AsyncWriteBufferOverflow: OSStatus

An asynchronous write operation could not be completed in time.

