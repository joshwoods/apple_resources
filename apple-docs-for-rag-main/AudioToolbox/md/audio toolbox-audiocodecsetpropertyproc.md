

- Audio Toolbox
-  AudioCodecSetPropertyProc 

Type Alias

# AudioCodecSetPropertyProc

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioCodecSetPropertyProc = (UnsafeMutableRawPointer, AudioCodecPropertyID, UInt32, UnsafeRawPointer) -> OSStatus
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

typealias AudioCodecGetPropertyProc

typealias AudioCodecInitializeProc

typealias AudioCodecProduceOutputBufferListProc

typealias AudioCodecProduceOutputPacketsProc

typealias AudioCodecPropertyID

An integer identifying an audio codec property.

typealias AudioCodecResetProc

typealias AudioCodecUninitializeProc

