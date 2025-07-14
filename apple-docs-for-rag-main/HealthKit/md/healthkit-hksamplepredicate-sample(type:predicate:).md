

- HealthKit
- HKSamplePredicate
-  sample(type:predicate:) 

Type Method

# sample(type:predicate:)

Returns a sample predicate that matches samples.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
static func sample(
    type sampleType: HKSampleType,
    predicate: NSPredicate? = nil
) -> HKSamplePredicate
```

## Parameters 

`sampleType`  

A type that matches samples.

`predicate`  

An optional predicate that further restricts the results that the query returns.

## Discussion

Use this method to create an HKSamplePredicate instance that you can use to query for a heterogenous set of sample types.

```
let stepType = HKQuantityType(.stepCount)
// Normally, you'd create a quantity predicate for step counts.
let stepPredicate = HKSamplePredicate.sample(type: stepType)

let highHeartRateType = HKCategoryType(.highHeartRateEvent)
// Normally, you'd create a category predicate for high heart rate events.
let highHeartRatePredicate = HKSamplePredicate.sample(type: highHeartRateType)

// By using sample predicates, you can query for different sample types.
let descriptor = HKSampleQueryDescriptor(
    predicates: [stepPredicate, highHeartRatePredicate],
    sortDescriptors: [],
    limit: 10)

// However, the results are an array of HKSample objects.
// You'll need to downcast them to access the data.
let results = try await descriptor.result(for: store)
```

## See Also

### Creating Sample Predicates

static func audiogram(NSPredicate?) -> HKSamplePredicate&lt;HKAudiogramSample>

Returns a sample predicate that matches audiogram samples.

static func categorySample(type: HKCategoryType, predicate: NSPredicate?) -> HKSamplePredicate&lt;HKCategorySample>

Returns a sample predicate that matches category samples.

static func clinicalRecord(type: HKClinicalType, predicate: NSPredicate?) -> HKSamplePredicate&lt;HKClinicalRecord>

Returns a sample predicate that matches clinical record samples.

static func correlation(type: HKCorrelationType, predicate: NSPredicate?) -> HKSamplePredicate&lt;HKCorrelation>

Returns a sample predicate that matches samples that contain correlated data.

static func electrocardiogram(NSPredicate?) -> HKSamplePredicate&lt;HKElectrocardiogram>

Returns a sample predicate that matches electrocardiogram samples.

static func heartbeatSeries(NSPredicate?) -> HKSamplePredicate&lt;HKHeartbeatSeriesSample>

Returns a sample predicate that matches heartbeat series samples.

static func quantitySample(type: HKQuantityType, predicate: NSPredicate?) -> HKSamplePredicate&lt;HKQuantitySample>

Returns a sample predicate that matches quantity samples.

static func visionPrescription(NSPredicate?) -> HKSamplePredicate&lt;HKVisionPrescription>

Returns a predicate that matches prescription samples.

static func workout(NSPredicate?) -> HKSamplePredicate&lt;HKWorkout>

Returns a sample predicate that matches workout samples.

static func workoutRoute(NSPredicate?) -> HKSamplePredicate&lt;HKWorkoutRoute>

Returns a sample predicate that matches samples containing workout route data.

