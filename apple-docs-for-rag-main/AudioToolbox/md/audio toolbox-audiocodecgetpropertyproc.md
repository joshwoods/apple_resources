

- Audio Toolbox
-  AudioCodecGetPropertyProc 

Type Alias

# AudioCodecGetPropertyProc

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioCodecGetPropertyProc = (UnsafeMutableRawPointer, AudioCodecPropertyID, UnsafeMutablePointer, UnsafeMutableRawPointer) -> OSStatus
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

typealias AudioCodecGetPropertyInfoProc

typealias AudioCodecInitializeProc

typealias AudioCodecProduceOutputBufferListProc

typealias AudioCodecProduceOutputPacketsProc

typealias AudioCodecPropertyID

An integer identifying an audio codec property.

typealias AudioCodecResetProc

typealias AudioCodecSetPropertyProc

typealias AudioCodecUninitializeProc

