

- Core Media
-  CMTime APIs 

API Collection

# CMTime APIs

A structure that represents time.

## Overview

Core Media represents time as a rational value, with a time value as the numerator and timescale as the denominator. The structure can represent a specific numeric time in the media timeline, and can also represent nonnumeric values like invalid and indefinite times or positive and negative infinity.

## Topics

### Creating a Time

func CMTimeMake(value: Int64, timescale: Int32) -> CMTime

Creates a time with a value and timescale.

func CMTimeMakeWithEpoch(value: Int64, timescale: Int32, epoch: Int64) -> CMTime

Creates a time with a value, timescale, and epoch.

func CMTimeMakeWithSeconds(Float64, preferredTimescale: Int32) -> CMTime

Creates a time that represents a number of seconds in a preferred timescale.

func CMTimeMakeFromDictionary(CFDictionary?) -> CMTime

Creates a time from a dictionary representation of its fields.

### Inspecting a Time

func CMTimeGetSeconds(CMTime) -> Float64

Returns a representation of the time in seconds.

func CMTimeAbsoluteValue(CMTime) -> CMTime

Returns the absolute value of a time.

func CMTIME_IS_VALID(CMTime) -> Bool

Returns a Boolean value that indicates whether a given time is valid.

func CMTIME_IS_INVALID(CMTime) -> Bool

Returns a Boolean value that indicates whether a given time is invalid.

func CMTIME_IS_POSITIVEINFINITY(CMTime) -> Bool

Returns a Boolean value that indicates whether a given time is positive infinity.

func CMTIME_IS_NEGATIVEINFINITY(CMTime) -> Bool

Returns a Boolean value that indicates whether a given time is negative infinity.

func CMTIME_IS_INDEFINITE(CMTime) -> Bool

Returns a Boolean value that indicates whether a given time is indefinite.

func CMTIME_IS_NUMERIC(CMTime) -> Bool

Returns a Boolean value that indicates whether a given time is numeric.

func CMTIME_HAS_BEEN_ROUNDED(CMTime) -> Bool

Returns a Boolean value that indicates whether the system rounded the time value.

### Performing Time Calculations

func CMTimeAdd(CMTime, CMTime) -> CMTime

Returns the sum of two times.

func CMTimeSubtract(CMTime, CMTime) -> CMTime

Returns the difference between two times.

func CMTimeMultiply(CMTime, multiplier: Int32) -> CMTime

Returns the result of multiplying a time by an integer multiplier.

func CMTimeMultiplyByFloat64(CMTime, multiplier: Float64) -> CMTime

Returns the result of multiplying a time by a floating-point multiplier.

func CMTimeMultiplyByRatio(CMTime, multiplier: Int32, divisor: Int32) -> CMTime

Returns the result of multiplying a time by an integer multiplier, and then dividing the result by the divisor.

### Changing the Timescale

func CMTimeConvertScale(CMTime, timescale: Int32, method: CMTimeRoundingMethod) -> CMTime

Converts the source time to a new timescale using the specified rounding method.

enum CMTimeRoundingMethod

An enumeration of rounding methods to use when performing time calculations.

### Comparing Times

func CMTimeCompare(CMTime, CMTime) -> Int32

Returns the numerical relationship of two times.

func CMTimeMaximum(CMTime, CMTime) -> CMTime

Returns the greater of two time values.

func CMTimeMinimum(CMTime, CMTime) -> CMTime

Returns the lesser of two time values.

### Representing Times

func CMTimeShow(CMTime)

Prints a description of the time to the console.

func CMTimeCopyDescription(allocator: CFAllocator?, time: CMTime) -> CFString?

Creates a string representation of the time.

func CMTimeCopyAsDictionary(CMTime, allocator: CFAllocator?) -> CFDictionary?

Creates a dictionary representation of the time.

### Data Types

struct CMTime

A structure that represents time.

typealias CMTimeValue

An integer time value.

typealias CMTimeScale

An integer timescale.

typealias CMTimeEpoch

An epoch for a time.

struct CMTimeFlags

A structure that defines the flags for a time value.

### Constants

Time

Defined time values.

Timescale

Defined timescale values.

Dictionary Keys

Keys to use when working with dictionary representations of time.

## See Also

### Time Representation

CMTimeRange APIs

A structure that represents a range of time.

CMTimeMapping APIs

A structure that maps a segment of a source time range to a target time range.

