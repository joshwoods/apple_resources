

- HealthKit
- HKStatistics
-  minimumQuantity() 

Instance Method

# minimumQuantity()

Returns the minimum value from all the samples that match the query.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func minimumQuantity() -> HKQuantity?
```

## Return Value

If the discreteMin option was set, this method returns a quantity object containing the minimum value from all the samples matching the query; otherwise, it returns `nil`.

## See Also

### Related Documentation

var endDate: Date

The end of the time period included in these statistics.

var startDate: Date

The start of the time period included in these statistics.

### Getting Statistics Data

func averageQuantity() -> HKQuantity?

Returns the average value from all the samples that match the query.

func averageQuantity(for: HKSource) -> HKQuantity?

Returns the average value from all the samples that match the query and that were created by the specified source.

func maximumQuantity() -> HKQuantity?

Returns the maximum value from all the samples that match the query.

func maximumQuantity(for: HKSource) -> HKQuantity?

Returns the maximum value from all the samples that match the query and that were created by the specified source.

func minimumQuantity(for: HKSource) -> HKQuantity?

Returns the minimum value from all the samples that match the query and that were created by the specified source.

func sumQuantity() -> HKQuantity?

Returns the sum of all the samples that match the query.

func sumQuantity(for: HKSource) -> HKQuantity?

Returns the sum of all the samples that match the query and that were created by the specified source.

func duration() -> HKQuantity?

Returns the total duration covering all the samples that match the query.

func duration(for: HKSource) -> HKQuantity?

Returns the total duration covering all the samples created by the specified source that also match the query.

