

- Core Media
- CMTimeRange
-  containsTime(\_:) 

Instance Method

# containsTime(\_:)

Returns a Boolean value that indicates whether the time range contains a time.

iOS 4.0+iPadOS 4.0+Mac CatalystmacOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func containsTime(_ time: CMTime) -> Bool
```

## Parameters 

`time`  

A time value to test for in the time range.

## Return Value

true if the time range contains the `time` value; otherwise, false.

## See Also

### Finding Elements

func containsTimeRange(CMTimeRange) -> Bool

Returns a Boolean value that indicates whether the time range contains another time range.

