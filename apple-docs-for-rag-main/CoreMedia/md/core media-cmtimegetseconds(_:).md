

- Core Media
-  CMTimeGetSeconds(\_:) 

Function

# CMTimeGetSeconds(\_:)

Returns a representation of the time in seconds.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeGetSeconds(_ time: CMTime) -> Float64
```

## Parameters 

`time`  

A time value for which to retrieve seconds.

## Return Value

The time in seconds.

## Discussion

If the time is invalid or indefinite, the result is nan.

If the time is infinite, the result is positive or negative infinity.

If the time is numeric, it ignores the epoch, and returns the result of `time.value / time.timescale`. It performs the division in `Float64`, so the fraction isn’t lost in the returned result.

## See Also

### Inspecting a Time

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

