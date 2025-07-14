

- Core Audio Types
-  AudioTimeStampFlags 

Structure

# AudioTimeStampFlags

A structure that represents flags for a timestamp.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
struct AudioTimeStampFlags
```

## Topics

### Initializers

init(rawValue: UInt32)

Creates a flag with an unsigned-integer value.

### Type Properties

static var hostTimeValid: AudioTimeStampFlags

A flag that indicates that the host time is valid.

static var rateScalarValid: AudioTimeStampFlags

A flag that indicates that the rate scalar is valid.

static var sampleHostTimeValid: AudioTimeStampFlags

A flag that indicates that the sample frame time and the host time are valid.

static var sampleTimeValid: AudioTimeStampFlags

A flag that indicates that the sample frame time is valid.

static var smpteTimeValid: AudioTimeStampFlags

A flag that indicates that the SMPTE time is valid.

static var wordClockTimeValid: AudioTimeStampFlags

A flag that indicates that the word clock time is valid.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Audio Time

struct AudioTimeStamp

A structure that represents a timestamp value.

