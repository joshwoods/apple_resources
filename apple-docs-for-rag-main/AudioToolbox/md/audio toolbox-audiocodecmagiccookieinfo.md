

- Audio Toolbox
-  AudioCodecMagicCookieInfo 

Structure

# AudioCodecMagicCookieInfo

A structure holding magic cookie information needed by some codecs.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioCodecMagicCookieInfo
```

## Overview

This structure is passed as input to the AudioCodecGetProperty(_:_:_:_:) function for the `kAudioCodecPropertyFormatList` property. The first `4 + sizeof(void *)` bytes of the buffer pointed to by the function’s `outPropertyData` parameter contains this structure on input.

## Topics

### Initializers

init()

init(mMagicCookieSize: UInt32, mMagicCookie: UnsafeRawPointer?)

### Instance Properties

var mMagicCookie: UnsafeRawPointer?

Generic constant pointer to the magic cookie.

var mMagicCookieSize: UInt32

The size of the magic cookie.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Codec Types

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

typealias AudioCodecSetPropertyProc

typealias AudioCodecUninitializeProc

