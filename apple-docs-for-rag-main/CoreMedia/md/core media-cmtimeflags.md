

- Core Media
-  CMTimeFlags 

Structure

# CMTimeFlags

A structure that defines the flags for a time value.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
struct CMTimeFlags
```

## Topics

### Properties

static var valid: CMTimeFlags

A flag that indicates a time is valid.

static var hasBeenRounded: CMTimeFlags

A flag that indicates a previous time calculation rounded the result.

static var positiveInfinity: CMTimeFlags

A flag that indicates the time is positive infinity.

static var negativeInfinity: CMTimeFlags

A flag that indicates the time is negative infinity.

static var indefinite: CMTimeFlags

A flag that indicates the time is indefinite.

static var impliedValueFlagsMask: CMTimeFlags

A flag that indicates the time is positive or negative infinity, or indefinite.

### Initializers

init(rawValue: UInt32)

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

### Data Types

struct CMTime

A structure that represents time.

typealias CMTimeValue

An integer time value.

typealias CMTimeScale

An integer timescale.

typealias CMTimeEpoch

An epoch for a time.

