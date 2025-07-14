

- Audio Toolbox
-  AudioCodecGetPropertyInfoProc 

Type Alias

# AudioCodecGetPropertyInfoProc

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioCodecGetPropertyInfoProc = (UnsafeMutableRawPointer, AudioCodecPropertyID, UnsafeMutablePointer?, UnsafeMutablePointer?) -> OSStatus
```

## See Also

### Codec Types

struct AudioCodecMagicCookieInfo

A structure holding magic cookie information needed by some codecs.

struct AudioCodecPrimeInfo

A structure specifying the number of leading and trailing empty frames to be inserted.

typealias AudioCodec

An instance of a Component Manager component.

typealias AudioCodecAppendInputBufferListProc

typealias AudioCodecAppendInputDataProc

typealias AudioCodecGetPropertyProc

typealias AudioCodecInitializeProc

typealias AudioCodecProduceOutputBufferListProc

typealias AudioCodecProduceOutputPacketsProc

typealias AudioCodecPropertyID

An integer identifying an audio codec property.

typealias AudioCodecResetProc

typealias AudioCodecSetPropertyProc

typealias AudioCodecUninitializeProc

