

- HealthKit
- HKCategorySample
-  init(type:value:start:end:) 

Initializer

# init(type:value:start:end:)

Creates a newly instantiated category sample.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    type: HKCategoryType,
    value: Int,
    start startDate: Date,
    end endDate: Date
)
```

## Parameters 

`type`  

The category type for this sample. For a complete list, see Category Type Identifiers in HealthKit Constants.

`value`  

The value for this sample. This value must come from the appropriate category value enumeration. Each category type uses its own enumeration. For more information, see Category Type Identifiers in HealthKit Constants.

`startDate`  

The start date for the sample. This must be equal to or earlier than the end date; otherwise, this method throws an exception (invalidArgumentException).

`endDate`  

The end date for the sample. This must be equal to or later than the start date; otherwise, this method throws an exception (invalidArgumentException).

## Return Value

A valid category sample.

## Discussion

HealthKit uses category samples to represent data that can be classified into a finite set of categories. To create a category sample, you must first create the corresponding category type, and then set its start and end dates, as shown below.

- Swift
- Objective-C

```
guard let categoryType =
    HKObjectType.categoryTypeForIdentifier(HKCategoryTypeIdentifierSleepAnalysis) else {
        fatalError("*** Unable to create a sleep analysis category type ***")
}

let categorySample = HKCategorySample(type: categoryType,
                                      value: HKCategoryValueSleepAnalysis.Asleep.rawValue,
                                      startDate: start,
                                      endDate: end)
```

```
HKCategoryType *categoryType =
[HKObjectType categoryTypeForIdentifier:HKCategoryTypeIdentifierSleepAnalysis];

HKCategorySample *categorySample =
[HKCategorySample categorySampleWithType:categoryType
                                   value:HKCategoryValueSleepAnalysisAsleep
                               startDate:start
                                 endDate:end];
```

## See Also

### Related Documentation

var value: Int

The category value for this sample.

class func categoryType(forIdentifier: HKCategoryTypeIdentifier) -> HKCategoryType?

Returns the shared category type for the provided identifier.

var endDate: Date

The sample’s end date.

var categoryType: HKCategoryType

The category type for this sample.

var startDate: Date

The sample’s start date.

### Creating Category Samples

convenience init(type: HKCategoryType, value: Int, start: Date, end: Date, metadata: [String : Any]?)

Creates a newly instantiated category sample with the provided metadata.

convenience init(type: HKCategoryType, value: Int, start: Date, end: Date, device: HKDevice?, metadata: [String : Any]?)

Creates a newly instantiated category sample including the provided device and metadata.

