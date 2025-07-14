

- HealthKit
- HKSample
-  sampleType 

Instance Property

# sampleType

The sample type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var sampleType: HKSampleType { get }
```

## Discussion

This property contains a concrete sample type that corresponds with this sample’s concrete class. For example, if the sample is an HKQuantitySample instance, it returns an HKQuantityType object.

## See Also

### Related Documentation

var quantityType: HKQuantityType

The quantity type for this sample.

var correlationType: HKCorrelationType

The type for this correlation.

var categoryType: HKCategoryType

The category type for this sample.

### Accessing the Sample’s Data

var startDate: Date

The sample’s start date.

var endDate: Date

The sample’s end date.

var hasUndeterminedDuration: Bool

Indicates whether the sample has an unknown duration.

