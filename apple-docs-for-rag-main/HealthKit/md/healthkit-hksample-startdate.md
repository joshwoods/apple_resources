

- HealthKit
- HKSample
-  startDate 

Instance Property

# startDate

The sample’s start date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var startDate: Date { get }
```

## Mentioned in 

Adding samples to a workout

Running workout sessions

## Discussion

The sample’s start date must be equal to or earlier than its end date.

Some samples—for example, body temperature—represent a single point in time. For these samples, both the start and the end date are the same, because they both refer to the point in time when the sample was taken.

Other samples—for example, step count—represent data over a time interval. Here, the sample should use different start and end dates. These dates mark the beginning and end of the sample’s time interval, respectively.

## See Also

### Accessing the Sample’s Data

var endDate: Date

The sample’s end date.

var hasUndeterminedDuration: Bool

Indicates whether the sample has an unknown duration.

var sampleType: HKSampleType

The sample type.

