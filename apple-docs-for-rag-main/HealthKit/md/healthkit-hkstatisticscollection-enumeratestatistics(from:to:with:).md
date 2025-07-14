

- HealthKit
- HKStatisticsCollection
-  enumerateStatistics(from:to:with:) 

Instance Method

# enumerateStatistics(from:to:with:)

Enumerates the statistics objects for all the time intervals from the start date until the end date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func enumerateStatistics(
    from startDate: Date,
    to endDate: Date,
    with block: @escaping (HKStatistics, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`startDate`  

The start date for the calculation. The initial statistics come from the time interval that contains the start date.

`endDate`  

The end date for the calculation. The final statistics come from the time interval that contains the end date.

`block`  

A block that is called once for each time interval. This method passes the following parameters to the block:

result  
The HKStatistics object containing the statistical data for this time interval.

stop  
A reference to a Boolean value. The block can set the value to true to stop further processing of the collection. The stop argument is an out-only argument. Only set this Boolean to true within the block.

## Discussion

This method enumerates the statistics in chronological order. It calls the block once for each time interval between the start and end dates. If there are no samples for a particular time interval, the corresponding statistic object has a `nil`-valued quantity.

## See Also

### Accessing Statistics Collections

func statistics() -> [HKStatistics]

Returns an array of statistics objects representing the populated time intervals covered by the statistics collection query.

func statistics(for: Date) -> HKStatistics?

Returns the statistics object for the time interval that contains the provided date.

