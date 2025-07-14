

- HealthKit
-  HKSamplePredicate 

Structure

# HKSamplePredicate

A predicate for queries that return a collection of matching sample objects.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct HKSamplePredicate where Sample : HKSample
```

## Overview

The HKSamplePredicate structure bundles an HKSampleType and an optional NSPredicate. The structure is generic. You can create it for any HKSampleType subclass, and it automatically sets the `Sample` type to the matching HKSampleType subtype. As a result, any query that you build using this structure returns properly typed results.

To create an HKSamplePredicate instance, call one of its constructor methods.

```
let stepType = HKQuantityType(.stepCount)
let predicate = HKSamplePredicate.quantitySample(type: stepType)

let descriptor = HKSampleQueryDescriptor(
    predicates:[predicate],
    sortDescriptors: [],
    limit: 10)

// The results are an array of HKQuantitySample objects.
let results = try await descriptor.result(for: store)
```

## Topics

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

static func visionPrescription(NSPredicate?) -> HKSamplePredicate&lt;HKVisionPrescription>

Returns a predicate that matches prescription samples.

static func workout(NSPredicate?) -> HKSamplePredicate&lt;HKWorkout>

Returns a sample predicate that matches workout samples.

static func workoutRoute(NSPredicate?) -> HKSamplePredicate&lt;HKWorkoutRoute>

Returns a sample predicate that matches samples containing workout route data.

### Accessing Sample Predicate Data

let nsPredicate: NSPredicate?

An optional predicate that further restricts the results that the query returns.

let sampleType: HKSampleType

The type of samples that the query returns.

### Type Methods

static func gad7Assessment(NSPredicate?) -> HKSamplePredicate&lt;HKGAD7Assessment>

static func phq9Assessment(NSPredicate?) -> HKSamplePredicate&lt;HKPHQ9Assessment>

static func stateOfMind(NSPredicate?) -> HKSamplePredicate&lt;HKStateOfMind>

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Swift concurrency support

Running Queries with Swift Concurrency

Use Swift concurrency to manage one-shot and long-running queries.

protocol HKAsyncQuery

A protocol that defines an asynchronous method for running queries.

protocol HKAsyncSequenceQuery

A protocol that defines a method for running queries that returns results using an asynchronous sequence.

