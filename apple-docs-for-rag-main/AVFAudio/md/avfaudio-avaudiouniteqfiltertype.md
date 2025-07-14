

- AVFAudio
-  AVAudioUnitEQFilterType 

Enumeration

# AVAudioUnitEQFilterType

Filter types available to use with the filter type property.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum AVAudioUnitEQFilterType
```

## Topics

### Filter Types

case parametric

A type that represents a parametric filter that derives from a Butterworth analog prototype.

case lowPass

A type that represents a simple Butterworth second-order low-pass filter.

case highPass

A type that represents a simple Butterworth second-order high-pass filter.

case resonantLowPass

A type that represents a low-pass filter with resonance support using the bandwidth parameter.

case resonantHighPass

A type that represents a high-pass filter with resonance support using the bandwidth parameter.

case bandPass

A type that represents a bandpass filter.

case bandStop

A type that represents a band-stop filter, also known as a notch filter.

case lowShelf

A type that represents a low-shelf filter.

case highShelf

A type that represents a high-shelf filter.

case resonantLowShelf

A type that represents a low-shelf filter with resonance support using the bandwidth parameter.

case resonantHighShelf

A type that represents a high-shelf filter with resonance support using the bandwidth parameter.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

