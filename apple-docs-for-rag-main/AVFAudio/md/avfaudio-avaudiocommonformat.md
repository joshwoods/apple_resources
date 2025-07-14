

- AVFAudio
-  AVAudioCommonFormat 

Enumeration

# AVAudioCommonFormat

The format options that describe common audio formats.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum AVAudioCommonFormat
```

## Topics

### Formats

case otherFormat

A format other than one the enumeration specifies.

case pcmFormatFloat32

A format that represents the standard format as native-endian floats.

case pcmFormatFloat64

A format that represents native-endian doubles.

case pcmFormatInt16

A format that represents signed 16-bit native-endian integers.

case pcmFormatInt32

A format that represents signed 32-bit native-endian integers.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

