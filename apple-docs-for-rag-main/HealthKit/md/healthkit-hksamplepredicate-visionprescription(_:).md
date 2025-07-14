

- HealthKit
- HKSamplePredicate
-  visionPrescription(\_:) 

Type Method

# visionPrescription(\_:)

Returns a predicate that matches prescription samples.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOSwatchOS 9.0+

``` source
static func visionPrescription(_ predicate: NSPredicate? = nil) -> HKSamplePredicate
```

Available when `Sample` inherits `HKSample`.

## Parameters 

`predicate`  

A predicate that further filters the matching prescriptions.

## Discussion

Use this method to create a predicate that matches vision prescriptions.

```
// Create a predicate that matches samples stored today.
let end = Date()
let start = Calendar.current.startOfDay(for: Date())
let datePredicate = HKQuery.predicateForSamples(withStart: start, end: end)

// Create a predicate that matches vision prescriptions samples stored today.
let predicate = HKSamplePredicate.visionPrescription(datePredicate)
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

static func sample(type: HKSampleType, predicate: NSPredicate?) -> HKSamplePredicate&lt;HKSample>

Returns a sample predicate that matches samples.

static func workout(NSPredicate?) -> HKSamplePredicate&lt;HKWorkout>

Returns a sample predicate that matches workout samples.

static func workoutRoute(NSPredicate?) -> HKSamplePredicate&lt;HKWorkoutRoute>

Returns a sample predicate that matches samples containing workout route data.

