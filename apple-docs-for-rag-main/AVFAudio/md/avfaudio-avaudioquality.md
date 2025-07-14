

- AVFAudio
-  AVAudioQuality 

Enumeration

# AVAudioQuality

The values that specify the sample rate audio quality for encoding and conversion.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum AVAudioQuality
```

## Overview

You use this value with AVEncoderAudioQualityKey and AVSampleRateConverterAudioQualityKey.

## Topics

### Constants

case min

A value that represents a minimum audio quality for encoding and conversion.

case low

A value that represents a low audio quality for encoding and conversion.

case medium

A value that represents a medium audio quality for encoding and conversion.

case high

A value that represents a high audio quality for encoding and conversion.

case max

A value that represents a maximum audio quality for encoding and conversion.

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

### Settings

Sample Rate Conversion Settings

The constants that define sample rate converter audio quality settings.

let AVEncoderAudioQualityKey: String

A constant that represents an integer from the audio quality enumeration.

Encoder Settings

The constants that define the audio encoder settings for the audio recorder class.

Time Pitch Algorithm Settings

The constants that define the values for the time pitch algorithms.

