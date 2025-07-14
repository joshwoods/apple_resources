

- Audio Toolbox
-  AudioBalanceFadeType 

Enumeration

# AudioBalanceFadeType

Identifiers for audio balance fade types.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum AudioBalanceFadeType
```

## Overview

These constants are used as values for the `mType` field of the AudioBalanceFade structure.

## Topics

### Types

case equalPower

Overall loudness remains constant, but gain can exceed 1.0. The gain value is 1.0 when the balance and fade are in the center. From there they can increase to +3dB (1.414) and decrease to silence.

case maxUnityGain

Ensures that the overall gain value never exceeds 1.0 by fading one channel as the other channel’s level rises. This can reduce overall loudness when the balance or fade is not in the center.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

Audio Format Property Identifiers

Constants for use with the AudioFormatGetPropertyInfo(_:_:_:_:) and AudioFormatGetProperty(_:_:_:_:_:) functions.

Audio Codec Component Constants

Audio codec component types.

Audio Codec Manufacturer and Implementation Types

Identifiers for audio codec manufacturers and implementation types.

enum AudioPanningMode

Identifiers for audio panning algorithms.

