

- HealthKit
- HKCategorySample
-  init(type:value:start:end:metadata:) 

Initializer

# init(type:value:start:end:metadata:)

Creates a newly instantiated category sample with the provided metadata.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    type: HKCategoryType,
    value: Int,
    start startDate: Date,
    end endDate: Date,
    metadata: [String : Any]?
)
```

## Parameters 

`type`  

The category type for this sample. For a complete list, see Category Type Identifiers in HealthKit Constants.

`value`  

The value for this sample. This value must come from the appropriate category value enumeration. Each category type uses its own enumeration. For more information, see Category Type Identifiers in HealthKit Constants.

`startDate`  

The start date for the sample. This must be equal to or earlier than the end date; otherwise, this method throws an exception (`NSInvalidArgumentException`).

`endDate`  

The end date for the sample. This must be equal to or later than the start date; otherwise, this method throws an exception (`NSInvalidArgumentException`).

`metadata`  

The metadata dictionary contains extra information describing this sample. The dictionary’s keys are all NSString objects. The values may be NSString objects, NSNumber objects or NSDate objects. For a complete list of predefined metadata keys, see Metadata Keys in HealthKit Constants.

Using predefined keys helps facilitate sharing data between apps; however, you are also encouraged to create your own, custom keys as needed to extend the HealthKit category sample’s capabilities.

## Return Value

A valid category sample with metadata.

## Discussion

HealthKit uses category samples to represent data that can be classified into a finite set of categories. To create a category sample, you must first create the corresponding category type and then set its start date, end date, and metadata, as shown below.

- Swift
- Objective-C

```
let metadata : [String : AnyObject] =
    [HKMetadataKeyDigitalSignature:digitalSignature,
     HKMetadataKeyTimeZone:timeZone]

guard let categoryType =
    HKObjectType.categoryTypeForIdentifier(HKCategoryTypeIdentifierSleepAnalysis) else {
        fatalError("*** Unable to create a sleep analysis category type ***")
}

let categorySample = HKCategorySample(type: categoryType,
                                      value: HKCategoryValueSleepAnalysis.Asleep.rawValue,
                                      startDate: start,
                                      endDate: end,
                                      metadata:metadata)
```

```
NSDictionary *metadata =
@{HKMetadataKeyDigitalSignature:digitalSignature,
HKMetadataKeyTimeZone:timeZone};

HKCategoryType *categoryType =
[HKObjectType categoryTypeForIdentifier:HKCategoryTypeIdentifierSleepAnalysis];

HKCategorySample *categorySample =
[HKCategorySample categorySampleWithType:categoryType
                                   value:HKCategoryValueSleepAnalysisAsleep
                               startDate:start
                                 endDate:end
                                metadata:metadata];
```

## See Also

### Related Documentation

var value: Int

The category value for this sample.

class func categoryType(forIdentifier: HKCategoryTypeIdentifier) -> HKCategoryType?

Returns the shared category type for the provided identifier.

var endDate: Date

The sample’s end date.

var metadata: [String : Any]?

The metadata for this HealthKit object.

var categoryType: HKCategoryType

The category type for this sample.

var startDate: Date

The sample’s start date.

### Creating Category Samples

convenience init(type: HKCategoryType, value: Int, start: Date, end: Date)

Creates a newly instantiated category sample.

convenience init(type: HKCategoryType, value: Int, start: Date, end: Date, device: HKDevice?, metadata: [String : Any]?)

Creates a newly instantiated category sample including the provided device and metadata.

