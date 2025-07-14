

- HealthKit
- HKStatisticsCollection
-  statistics(for:) 

Instance Method

# statistics(for:)

Returns the statistics object for the time interval that contains the provided date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func statistics(for date: Date) -> HKStatistics?
```

## Parameters 

`date`  

The target date.

## Return Value

A statistics object for the time interval containing the provided date. If there are no samples for the selected time interval, the statistics object has a `nil`-valued quantity.

## See Also

### Accessing Statistics Collections

func statistics() -> [HKStatistics]

Returns an array of statistics objects representing the populated time intervals covered by the statistics collection query.

func enumerateStatistics(from: Date, to: Date, with: (HKStatistics, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates the statistics objects for all the time intervals from the start date until the end date.

