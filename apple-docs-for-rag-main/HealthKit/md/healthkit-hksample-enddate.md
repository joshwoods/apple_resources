

- HealthKit
- HKSample
-  endDate 

Instance Property

# endDate

The sample’s end date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var endDate: Date { get }
```

## Mentioned in 

Adding samples to a workout

## Discussion

The sample’s end date must be equal to or later than its start date.

Some samples—for example, body temperature—represent a single point in time. For these samples, both the start and the end date are the same, because they both refer to the point in time when the sample was taken.

Other samples—for example, step count—represent data over a time interval. Here, the sample should use different start and end dates. These dates mark the beginning and end of the sample’s time interval, respectively.

## See Also

### Accessing the Sample’s Data

var startDate: Date

The sample’s start date.

var hasUndeterminedDuration: Bool

Indicates whether the sample has an unknown duration.

var sampleType: HKSampleType

The sample type.

