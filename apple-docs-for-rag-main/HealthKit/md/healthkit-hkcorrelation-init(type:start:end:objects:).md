

- HealthKit
- HKCorrelation
-  init(type:start:end:objects:) 

Initializer

# init(type:start:end:objects:)

Instantiates and returns a new correlation instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    type correlationType: HKCorrelationType,
    start startDate: Date,
    end endDate: Date,
    objects: Set
)
```

## Parameters 

`correlationType`  

The type for this correlation. For a complete list of correlation types, see Correlation Identifiers in HealthKit Constants.

`startDate`  

The start date for the sample. This date must be equal to or earlier than the end date; otherwise, this method throws an exception (invalidArgumentException).

`endDate`  

The end date for the sample. This date must be equal to or later than the start date; otherwise, this method throws an exception (invalidArgumentException).

`objects`  

A set of HKSample objects. Specifically, this set contains the quantity and category samples to be grouped into this correlation.

## Return Value

A new correlation instance.

## Discussion

Use a correlation object to represent composite data—that is, a sample that requires more than a single value. To create a correlation sample, first create the quantity and category samples you intend to combine into the correlation. Next, create the correlation’s type. Finally, instantiate the correlation, passing in the type, start date, end date, and samples, as shown below.

Use this method when you do not need to include additional metadata and the data was not recorded using external hardware.

- Swift
- Objective-C

```
let date = NSDate()

// Create systolic sample

guard let systolicType = HKObjectType.quantityTypeForIdentifier(HKQuantityTypeIdentifierBloodPressureSystolic) else {
    fatalError("*** Unable to create the systolic type ****")
}

let systolicQuantity =
    HKQuantity(unit: HKUnit.millimeterOfMercuryUnit(), doubleValue: 120.0)

let systolicSample = HKQuantitySample(type: systolicType,
                                      quantity: systolicQuantity, startDate: date, endDate: date)

// Create diastolic sample

guard let diastolicType = HKObjectType.quantityTypeForIdentifier(HKQuantityTypeIdentifierBloodPressureDiastolic) else {
    fatalError("*** Unable to create the diastolic type ***")
}

let diastolicQuantity =
    HKQuantity(unit: HKUnit.millimeterOfMercuryUnit(), doubleValue: 75.0)

let diastolicSample = HKQuantitySample(type: diastolicType,
                                       quantity: diastolicQuantity, startDate: date, endDate: date)

// Create blood pressure sample

guard let bloodPressureType = HKObjectType.correlationTypeForIdentifier(HKCorrelationTypeIdentifierBloodPressure) else {
    fatalError("*** Unable to create the blood pressure type ***")
}

let objects: Set = [systolicSample, diastolicSample]

let bloodpressure = HKCorrelation(type: bloodPressureType,
                                  startDate: date, endDate: date, objects:objects)
```

```
NSDate *date = [NSDate date];

// Create systolic sample

HKQuantityType *systolicType =
[HKObjectType quantityTypeForIdentifier:
     HKQuantityTypeIdentifierBloodPressureSystolic];

HKQuantity *systolicQuantity =
[HKQuantity quantityWithUnit:[HKUnit millimeterOfMercuryUnit]
                 doubleValue:120.0];

HKQuantitySample *systolicSample =
[HKQuantitySample quantitySampleWithType:systolicType
                                quantity:systolicQuantity
                               startDate:date
                                 endDate:date];

// Create diastolic sample

HKQuantityType *diastolicType =
[HKObjectType quantityTypeForIdentifier:
    HKQuantityTypeIdentifierBloodPressureDiastolic];

HKQuantity *diastolicQuantity =
[HKQuantity quantityWithUnit:[HKUnit millimeterOfMercuryUnit]
                 doubleValue:75.0];

HKQuantitySample *diastolicSample =
[HKQuantitySample quantitySampleWithType:diastolicType
                                quantity:diastolicQuantity
                               startDate:date
                                 endDate:date];

// Create blood pressure sample

HKCorrelationType *bloodPressureType =
[HKObjectType correlationTypeForIdentifier:
    HKCorrelationTypeIdentifierBloodPressure];

NSSet *objects = [NSSet setWithObjects:systolicSample, diastolicSample, nil];

HKCorrelation *bloodPressure =
[HKCorrelation correlationWithType:bloodPressureType
                         startDate:date
                           endDate:date
                           objects:objects];
```

## See Also

### Related Documentation

var objects: Set&lt;HKSample>

The set of sample objects that make up the correlation.

class func correlationType(forIdentifier: HKCorrelationTypeIdentifier) -> HKCorrelationType?

Returns the shared correlation type for the provided identifier.

var endDate: Date

The sample’s end date.

var correlationType: HKCorrelationType

The type for this correlation.

var metadata: [String : Any]?

The metadata for this HealthKit object.

var startDate: Date

The sample’s start date.

### Creating Correlations

convenience init(type: HKCorrelationType, start: Date, end: Date, objects: Set&lt;HKSample>, metadata: [String : Any]?)

Instantiates and returns a new correlation instance with the provided metadata.

convenience init(type: HKCorrelationType, start: Date, end: Date, objects: Set&lt;HKSample>, device: HKDevice?, metadata: [String : Any]?)

Instantiates and returns a new correlation instance with the provided device and metadata.

