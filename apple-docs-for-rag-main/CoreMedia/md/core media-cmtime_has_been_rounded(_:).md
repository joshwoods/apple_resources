

- Core Media
-  CMTIME_HAS_BEEN_ROUNDED(\_:) 

Function

# CMTIME_HAS_BEEN_ROUNDED(\_:)

Returns a Boolean value that indicates whether the system rounded the time value.

iOS 4.0+iPadOS 4.0+Mac CatalystmacOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTIME_HAS_BEEN_ROUNDED(_ time: CMTime) -> Bool
```

## Parameters 

`time`  

A time value to test.

## Return Value

true if the time represents a rounded value; otherwise, false.

## See Also

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

