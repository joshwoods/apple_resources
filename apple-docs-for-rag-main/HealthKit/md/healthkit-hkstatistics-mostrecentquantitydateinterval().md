

- HealthKit
- HKStatistics
-  mostRecentQuantityDateInterval() 

Instance Method

# mostRecentQuantityDateInterval()

Returns the date interval of the most recent sample that matches the query.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.0+

``` source
func mostRecentQuantityDateInterval() -> DateInterval?
```

## See Also

### Related Documentation

static var discreteMostRecent: HKStatisticsOptions

An option indicating that the system returns the most recent quantity from the matching samples.

Deprecated

### Getting the Most Recent Quantity

func mostRecentQuantity() -> HKQuantity?

Returns the most recent value from all the samples that match the query.

func mostRecentQuantity(for: HKSource) -> HKQuantity?

Returns the most recent value from all the samples that match the query and were created by the specified source.

func mostRecentQuantityDateInterval(for: HKSource) -> DateInterval?

Returns the date interval of the most recent sample that matches the query and was created by the specified source.

