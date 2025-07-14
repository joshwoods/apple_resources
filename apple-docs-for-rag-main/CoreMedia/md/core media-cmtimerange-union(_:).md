

- Core Media
- CMTimeRange
-  union(\_:) 

Instance Method

# union(\_:)

Returns a new time range with the time elements of both this time range and the given time range.

iOS 4.0+iPadOS 4.0+Mac CatalystmacOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func union(_ otherRange: CMTimeRange) -> CMTimeRange
```

## Parameters 

`otherRange`  

A time range.

## Return Value

A time range with the unique time elements of this time range and the input.

## See Also

### Combining Time Ranges

func intersection(CMTimeRange) -> CMTimeRange

Returns a new time range with the time elements that are common to both this time range and the given time range.

