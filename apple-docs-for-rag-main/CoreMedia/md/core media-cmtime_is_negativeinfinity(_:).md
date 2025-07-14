

- Core Media
-  CMTIME_IS_NEGATIVEINFINITY(\_:) 

Function

# CMTIME_IS_NEGATIVEINFINITY(\_:)

Returns a Boolean value that indicates whether a given time is negative infinity.

iOS 4.0+iPadOS 4.0+Mac CatalystmacOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTIME_IS_NEGATIVEINFINITY(_ time: CMTime) -> Bool
```

## Parameters 

`time`  

A time value to test.

## Return Value

true if the time represents negative infinity; otherwise, false.

## Discussion

Use this macro instead of testing whether a time is equal to negativeInfinity, because there are many times that negative positive infinity. This is because the system ignores nonflags fields, so they can contain anything.

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

func CMTIME_IS_INDEFINITE(CMTime) -> Bool

Returns a Boolean value that indicates whether a given time is indefinite.

func CMTIME_IS_NUMERIC(CMTime) -> Bool

Returns a Boolean value that indicates whether a given time is numeric.

func CMTIME_HAS_BEEN_ROUNDED(CMTime) -> Bool

Returns a Boolean value that indicates whether the system rounded the time value.

