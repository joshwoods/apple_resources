

- HealthKit
- HKQuantitySample
-  init(type:quantity:start:end:metadata:) 

Initializer

# init(type:quantity:start:end:metadata:)

Returns a sample containing a numeric measurement with the provided metadata.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    type quantityType: HKQuantityType,
    quantity: HKQuantity,
    start startDate: Date,
    end endDate: Date,
    metadata: [String : Any]?
)
```

## Parameters 

`quantityType`  

The type of sample to be created. HealthKit defines a number of different quantity types, representing different types of health and fitness data. For the complete list of quantity type identifiers, see HKQuantityTypeIdentifier.

`quantity`  

The value to be stored in the sample. The quantity object must use units that are compatible with the provided quantity type. If the units are not compatible, this method throws an exception (invalidArgumentException).

`startDate`  

The start date for the sample. This date must be equal to or earlier than the end date; otherwise, this method throws an exception (invalidArgumentException).

`endDate`  

The end date for the sample. This date must be equal to or later than the start date; otherwise, this method throws an exception (invalidArgumentException).

`metadata`  

The metadata dictionary contains extra information describing this sample. The dictionary’s keys are all NSString objects. The values may be NSString objects, NSNumber objects, or NSDate objects. For a complete list of predefined metadata keys, see Metadata Keys.

Using predefined keys helps facilitate sharing data between apps; however, you are also encouraged to create your own, custom keys as needed to extend the HealthKit quantity sample’s capabilities.

## Return Value

A valid quantity sample with metadata.

## Discussion

HealthKit uses quantity samples to represent sample data using a single numeric value. To create a quantity sample, first create the corresponding quantity type and quantity, and then set its start date, end date, and metadata. You produce a new quantity sample with the provided metadata.

- Swift
- Objective-C

```
let metadata = [HKMetadataKeyDigitalSignature:digitalSignature,
                HKMetadataKeyTimeZone:timeZone]

guard let quantityType = HKObjectType.quantityTypeForIdentifier(HKQuantityTypeIdentifierHeartRate) else {
    fatalError("*** Unable to create a heart rate quantity type ***")
}

let bpm = HKUnit(fromString: "count/min")
let quantity = HKQuantity(unit: bpm, doubleValue: 72.0)

let quantitySample = HKQuantitySample(type: quantityType,
                                      quantity: quantity,
                                      startDate: start,
                                      endDate: end,
                                      metadata: metadata)
```

```
NSDictionary *metadata =
@{HKMetadataKeyDigitalSignature:digitalSignature,
HKMetadataKeyTimeZone:timeZone};

HKQuantityType *quantityType =
[HKObjectType quantityTypeForIdentifier:HKQuantityTypeIdentifierHeartRate];

HKUnit *bpm = [HKUnit unitFromString:@"count/min"];

HKQuantity *quantity = [HKQuantity quantityWithUnit:bpm
                                        doubleValue:72.0];

HKQuantitySample *sample =
[HKQuantitySample quantitySampleWithType:quantityType
                                quantity:quantity
                               startDate:start
                                 endDate:end
                                metadata:metadata];
```

## See Also

### Related Documentation

var quantityType: HKQuantityType

The quantity type for this sample.

var quantity: HKQuantity

The quantity for this sample.

var endDate: Date

The sample’s end date.

var metadata: [String : Any]?

The metadata for this HealthKit object.

class func quantityType(forIdentifier: HKQuantityTypeIdentifier) -> HKQuantityType?

Returns the shared quantity type for the provided identifier.

var startDate: Date

The sample’s start date.

### Creating Quantity Samples

convenience init(type: HKQuantityType, quantity: HKQuantity, start: Date, end: Date)

Returns a sample containing a numeric measurement.

convenience init(type: HKQuantityType, quantity: HKQuantity, start: Date, end: Date, device: HKDevice?, metadata: [String : Any]?)

Returns a sample containing a numeric measurement with the provided device and metadata.

