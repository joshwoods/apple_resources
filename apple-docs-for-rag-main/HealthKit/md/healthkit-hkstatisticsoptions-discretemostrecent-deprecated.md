

- HealthKit
- HKStatisticsOptions
-  discreteMostRecent Deprecated

Type Property

# discreteMostRecent

An option indicating that the system returns the most recent quantity from the matching samples.

iOS 12.0–13.0DeprecatediPadOS 12.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 13.0+visionOS 1.0–1.0DeprecatedwatchOS 5.0–6.0Deprecated

``` source
static var discreteMostRecent: HKStatisticsOptions { get }
```

Deprecated

Use mostRecent instead.

## See Also

### Related Documentation

func mostRecentQuantity() -> HKQuantity?

Returns the most recent value from all the samples that match the query.

func mostRecentQuantity(for: HKSource) -> HKQuantity?

Returns the most recent value from all the samples that match the query and were created by the specified source.

func mostRecentQuantityDateInterval() -> DateInterval?

Returns the date interval of the most recent sample that matches the query.

func mostRecentQuantityDateInterval(for: HKSource) -> DateInterval?

Returns the date interval of the most recent sample that matches the query and was created by the specified source.

