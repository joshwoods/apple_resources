

- Audio Toolbox
-  AudioCodecPrimeInfo 

Structure

# AudioCodecPrimeInfo

A structure specifying the number of leading and trailing empty frames to be inserted.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioCodecPrimeInfo
```

## Topics

### Initializers

init()

init(leadingFrames: UInt32, trailingFrames: UInt32)

### Instance Properties

var leadingFrames: UInt32

An unsigned integer specifying the number of leading empty frames.

var trailingFrames: UInt32

An unsigned integer specifying the number of trailing empty frames.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Codec Types

struct AudioCodecMagicCookieInfo

A structure holding magic cookie information needed by some codecs.

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

typealias AudioCodecSetPropertyProc

typealias AudioCodecUninitializeProc

