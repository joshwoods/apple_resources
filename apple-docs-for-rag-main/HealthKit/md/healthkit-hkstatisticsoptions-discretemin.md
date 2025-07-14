

- HealthKit
- HKStatisticsOptions
-  discreteMin 

Type Property

# discreteMin

An option indicating that the system calculates the minimum quantity for the samples.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
static var discreteMin: HKStatisticsOptions { get }
```

## See Also

### Constants

static var separateBySource: HKStatisticsOptions

An option indicating that the system calculates the specified statistics separately for each source.

static var discreteAverage: HKStatisticsOptions

An option indicating that the system calculates the average quantity for the samples.

static var discreteMax: HKStatisticsOptions

An option indicating that the system calculates the maximum quantity for the samples.

static var cumulativeSum: HKStatisticsOptions

An option indicating that the system calculates the sum of all the quantities for the samples.

static var mostRecent: HKStatisticsOptions

An option indicating that the system returns the most recent quantity from the matching samples.

static var duration: HKStatisticsOptions

An option indicating that the system calculates the total duration covering all the samples.

