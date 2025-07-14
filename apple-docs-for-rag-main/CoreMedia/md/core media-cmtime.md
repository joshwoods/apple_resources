

- Core Media
-  CMTime 

Structure

# CMTime

A structure that represents time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
struct CMTime
```

## Overview

Core Media represents time as a rational value, with a time value as the numerator and timescale as the denominator. The structure can represent a specific numeric time in the media timeline, and can also represent nonnumeric values like invalid and indefinite times or positive and negative infinity.

## Topics

### Creating a Time

init(value: CMTimeValue, timescale: CMTimeScale)

Creates a time with a value and timescale.

init(value: CMTimeValue, timescale: CMTimeScale, flags: CMTimeFlags, epoch: CMTimeEpoch)

Creates a time with a value, timescale, flags, and epoch.

init(seconds: Double, preferredTimescale: CMTimeScale)

Creates a time that represents number of seconds in a preferred timescale.

init()

Creates a time with an invalid value.

### Inspecting a Time

var seconds: Double

A representation of the time in seconds.

var hasBeenRounded: Bool

A Boolean value that indicates whether the system rounded the time.

var isValid: Bool

A Boolean value that indicates whether a time is valid.

var isNumeric: Bool

A Boolean value that indicates whether a time is numeric.

var isIndefinite: Bool

A Boolean value that indicates whether a time is indefinite.

var isPositiveInfinity: Bool

A Boolean value that indicates whether a time represents positive infinity.

var isNegativeInfinity: Bool

A Boolean value that indicates whether a time represents negative infinity.

### Performing Time Calcualtions

static func + (CMTime, CMTime) -> CMTime

Returns a new time that represents the sum of two times.

static func - (CMTime, CMTime) -> CMTime

Returns a new time that represents the difference between two times.

### Changing the Timescale

func convertScale(Int32, method: CMTimeRoundingMethod) -> CMTime

Converts the source time to a new timescale using the specified rounding method.

enum CMTimeRoundingMethod

An enumeration of rounding methods to use when performing time calculations.

### Accessing Time Values

var value: CMTimeValue

A time value that represents the numerator of a rational time.

var timescale: CMTimeScale

A timescale that represents the denominator of a rational time.

var flags: CMTimeFlags

The flags associated with a time.

var epoch: CMTimeEpoch

The epoch of the time.

### Constants

static let zero: CMTime

A value that represents time zero.

static let invalid: CMTime

A value that represents an invalid time.

static let indefinite: CMTime

A value that represents an indefinite time.

static let negativeInfinity: CMTime

A value that represents negative infinity.

static let positiveInfinity: CMTime

A value that represents positive infinity.

### Operators

static func != (CMTime, CMTime) -> Bool

## Relationships

### Conforms To

- BitwiseCopyable
- Comparable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Data Types

typealias CMTimeValue

An integer time value.

typealias CMTimeScale

An integer timescale.

typealias CMTimeEpoch

An epoch for a time.

struct CMTimeFlags

A structure that defines the flags for a time value.

