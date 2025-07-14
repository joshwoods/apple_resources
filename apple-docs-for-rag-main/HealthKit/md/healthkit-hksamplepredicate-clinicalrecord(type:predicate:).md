

- HealthKit
- HKSamplePredicate
-  clinicalRecord(type:predicate:) 

Type Method

# clinicalRecord(type:predicate:)

Returns a sample predicate that matches clinical record samples.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOS

``` source
static func clinicalRecord(
    type clinicalType: HKClinicalType,
    predicate: NSPredicate? = nil
) -> HKSamplePredicate
```

## Parameters 

`clinicalType`  

A type that matches samples that contain clinical record data.

`predicate`  

An optional predicate that further restricts the results that the query returns.

## Discussion

Use this method to create an HKSamplePredicate instance that you can use to query for HKClinicalRecord objects.

## See Also

### Creating Sample Predicates

static func audiogram(NSPredicate?) -> HKSamplePredicate&lt;HKAudiogramSample>

Returns a sample predicate that matches audiogram samples.

static func categorySample(type: HKCategoryType, predicate: NSPredicate?) -> HKSamplePredicate&lt;HKCategorySample>

Returns a sample predicate that matches category samples.

static func correlation(type: HKCorrelationType, predicate: NSPredicate?) -> HKSamplePredicate&lt;HKCorrelation>

Returns a sample predicate that matches samples that contain correlated data.

static func electrocardiogram(NSPredicate?) -> HKSamplePredicate&lt;HKElectrocardiogram>

Returns a sample predicate that matches electrocardiogram samples.

static func heartbeatSeries(NSPredicate?) -> HKSamplePredicate&lt;HKHeartbeatSeriesSample>

Returns a sample predicate that matches heartbeat series samples.

static func quantitySample(type: HKQuantityType, predicate: NSPredicate?) -> HKSamplePredicate&lt;HKQuantitySample>

Returns a sample predicate that matches quantity samples.

static func sample(type: HKSampleType, predicate: NSPredicate?) -> HKSamplePredicate&lt;HKSample>

Returns a sample predicate that matches samples.

static func visionPrescription(NSPredicate?) -> HKSamplePredicate&lt;HKVisionPrescription>

Returns a predicate that matches prescription samples.

static func workout(NSPredicate?) -> HKSamplePredicate&lt;HKWorkout>

Returns a sample predicate that matches workout samples.

static func workoutRoute(NSPredicate?) -> HKSamplePredicate&lt;HKWorkoutRoute>

Returns a sample predicate that matches samples containing workout route data.

