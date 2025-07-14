

- HealthKit
- HKSamplePredicate
-  electrocardiogram(\_:) 

Type Method

# electrocardiogram(\_:)

Returns a sample predicate that matches electrocardiogram samples.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
static func electrocardiogram(_ predicate: NSPredicate? = nil) -> HKSamplePredicate
```

## Parameters 

`predicate`  

An optional predicate that further restricts the results that the query returns.

## Discussion

Use this method to create an HKSamplePredicate instance that you can use to query for HKElectrocardiogram objects.

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

