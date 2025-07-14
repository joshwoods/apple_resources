

- HealthKit
- HKSample
-  hasUndeterminedDuration 

Instance Property

# hasUndeterminedDuration

Indicates whether the sample has an unknown duration.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+macOS 13.0+visionOS 1.0+watchOS 7.2+

``` source
var hasUndeterminedDuration: Bool { get }
```

## Discussion

This property is true if the sample’s endDate property is distantFuture.

## See Also

### Accessing the Sample’s Data

var startDate: Date

The sample’s start date.

var endDate: Date

The sample’s end date.

var sampleType: HKSampleType

The sample type.

