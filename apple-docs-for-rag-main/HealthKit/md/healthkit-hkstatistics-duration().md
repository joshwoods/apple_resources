

- HealthKit
- HKStatistics
-  duration() 

Instance Method

# duration()

Returns the total duration covering all the samples that match the query.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func duration() -> HKQuantity?
```

## Discussion

If you set the duration option, this method returns a quantity object containing total duration covering all the samples that match the query; otherwise, it returns `nil`.

## See Also

### Getting Statistics Data

func averageQuantity() -> HKQuantity?

Returns the average value from all the samples that match the query.

func averageQuantity(for: HKSource) -> HKQuantity?

Returns the average value from all the samples that match the query and that were created by the specified source.

func maximumQuantity() -> HKQuantity?

Returns the maximum value from all the samples that match the query.

func maximumQuantity(for: HKSource) -> HKQuantity?

Returns the maximum value from all the samples that match the query and that were created by the specified source.

func minimumQuantity() -> HKQuantity?

Returns the minimum value from all the samples that match the query.

func minimumQuantity(for: HKSource) -> HKQuantity?

Returns the minimum value from all the samples that match the query and that were created by the specified source.

func sumQuantity() -> HKQuantity?

Returns the sum of all the samples that match the query.

func sumQuantity(for: HKSource) -> HKQuantity?

Returns the sum of all the samples that match the query and that were created by the specified source.

func duration(for: HKSource) -> HKQuantity?

Returns the total duration covering all the samples created by the specified source that also match the query.

