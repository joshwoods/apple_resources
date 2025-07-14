

- Core Media
-  CMTimeMinimum(\_:\_:) 

Function

# CMTimeMinimum(\_:\_:)

Returns the lesser of two time values.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeMinimum(
    _ time1: CMTime,
    _ time2: CMTime
) -> CMTime
```

## Parameters 

`time1`  

A time value.

`time2`  

Another time value.

## Return Value

The lesser of the two times.

## See Also

### Comparing Times

func CMTimeCompare(CMTime, CMTime) -> Int32

Returns the numerical relationship of two times.

func CMTimeMaximum(CMTime, CMTime) -> CMTime

Returns the greater of two time values.

