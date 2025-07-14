

- Foundation
- NSDateInterval
-  intersection(with:) 

Instance Method

# intersection(with:)

Returns the intersection between the receiver and the specified date interval.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func intersection(with dateInterval: DateInterval) -> DateInterval?
```

## Parameters 

`dateInterval`  

The date interval with which to calculate the intersection of the receiver.

## Return Value

A date interval for the intersection of the receiver and `dateInterval`, or `nil` if no intersection occurs.

## Discussion

Calculating the intersection of date intervals is a commutative and associative operation. The intersection of a date interval with itself is equal to itself.

The following figure illustrates five `NSDateInterval` objects plotted on an arbitrary time axis. Each date interval spans its duration from left to right, from its startDate to its endDate.

The date intervals labeled **A** and **B** do not intersect, because the startDate of **B** occurs later than the endDate of **A**.

The date intervals labeled **C** and **D** do intersect. The date interval labeled **E** represents the result of calculating the intersection between **C** and **D**.

## See Also

### Determining Intersections

func intersects(DateInterval) -> Bool

Indicates whether the receiver intersects with the specified date interval.

