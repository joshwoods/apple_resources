

- Audio Toolbox
-  AudioCodecInitializeProc 

Type Alias

# AudioCodecInitializeProc

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioCodecInitializeProc = (UnsafeMutableRawPointer, UnsafePointer?, UnsafePointer?, UnsafeRawPointer?, UInt32) -> OSStatus
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

typealias AudioCodecProduceOutputBufferListProc

typealias AudioCodecProduceOutputPacketsProc

typealias AudioCodecPropertyID

An integer identifying an audio codec property.

typealias AudioCodecResetProc

typealias AudioCodecSetPropertyProc

typealias AudioCodecUninitializeProc

