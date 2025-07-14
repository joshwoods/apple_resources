

- AVFAudio
-  AVAudioConverterPrimeMethod 

Enumeration

# AVAudioConverterPrimeMethod

Options for the prime method property.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum AVAudioConverterPrimeMethod
```

## Overview

For more information, see AVAudioConverterPrimeInfo.

## Topics

### Options

case pre

An option to prime with leading and trailing input frames.

case normal

An option to prime with trailing (zero latency) frames where the converter assumes the leading frames are silence.

case none

An option to prime the converter assumes leading and trailing frames are silence.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Priming Information

var primeInfo: AVAudioConverterPrimeInfo

The number of priming frames the converter uses.

var primeMethod: AVAudioConverterPrimeMethod

The priming method the sample rate converter or decoder uses.

struct AVAudioConverterPrimeInfo

Priming information for audio conversion.

