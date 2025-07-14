

- HealthKit
-  HKQuery 

Class

# HKQuery

An abstract class for all the query classes in HealthKit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKQuery
```

## Mentioned in 

Dividing a HealthKit workout into activities

## Overview

The HKQuery class is the basis for all the query objects that retrieve data from the HealthKit store. The HKQuery class is an abstract class. You should never instantiate it directly. Instead, you always work with one of its concrete subclasses.

### Filter queries using predicates

All the concrete `HKQuery` subclasses take a predicate. You can use this predicate to filter the samples returned by the query. When HealthKit runs a query, it converts the predicate to SQL and executes the SQL on the underlying store. This has two important side effects.

- Predicates improve the performance of your query, both in terms of speed and memory usage. Because the store executes the predicate, it restricts the number of HealthKit objects that it instantiates and returns.

- Since the store executes these predicates, it limits the type of predicates that you can use. Specifically, HealthKit provides several predicate key paths (for example, HKPredicateKeyPathUUID and HKPredicateKeyPathMetadata). You can create predicates using only these key paths.

## Topics

### Accessing properties

var predicate: NSPredicate?

A predicate used to filter the objects returned from the HealthKit store.

var objectType: HKObjectType?

The type of objects being queried.

var sampleType: HKSampleType?

The type of objects being queried.

Deprecated

### Creating object predicates

class func predicateForObject(with: UUID) -> NSPredicate

Returns a predicate that matches an object with the specified universally unique identifier (UUID).

class func predicateForObjects(with: Set&lt;UUID>) -> NSPredicate

Returns a predicate that matches the objects with the specified universally unique identifiers (UUIDs).

class func predicateForObjects(from: HKSource) -> NSPredicate

Returns a predicate that matches all the objects that were created by the provided source.

class func predicateForObjects(from: Set&lt;HKSource>) -> NSPredicate

Returns a predicate that matches all the objects that were created by any of the provided sources.

class func predicateForObjects(from: Set&lt;HKDevice>) -> NSPredicate

Returns a predicate that matches all the objects that were created by any of the provided devices.

class func predicateForObjects(withDeviceProperty: String, allowedValues: Set&lt;String>) -> NSPredicate

Returns a predicate that matches all objects created by devices with the specified properties.

class func predicateForObjects(from: Set&lt;HKSourceRevision>) -> NSPredicate

Returns a predicate that matches all the objects that were created by any of the provided source revisions.

class func predicateForObjects(withMetadataKey: String) -> NSPredicate

Returns a predicate that matches any object whose metadata contains the provided key.

class func predicateForObjects(withMetadataKey: String, allowedValues: [Any]) -> NSPredicate

Returns a predicate that matches objects based on the provided metadata key and an array of target values.

class func predicateForObjects(withMetadataKey: String, operatorType: NSComparisonPredicate.Operator, value: Any) -> NSPredicate

Returns a predicate that matches objects based on the provided metadata key, value, and operator.

class func predicateForObjectsWithNoCorrelation() -> NSPredicate

Returns a predicate that matches all objects that are not associated with a HealthKit correlation.

### Creating sample predicates

class func predicateForSamples(withStart: Date?, end: Date?, options: HKQueryOptions) -> NSPredicate

Returns a predicate for samples whose start and end dates fall within the specified time interval.

struct HKQueryOptions

Constants that describe how a sample’s time period overlaps with the target time period.

### Creating quantity sample predicates

class func predicateForQuantitySamples(with: NSComparisonPredicate.Operator, quantity: HKQuantity) -> NSPredicate

Returns a predicate that matches samples based on the target quantity.

### Creating category sample predicates

class func predicateForCategorySamples(with: NSComparisonPredicate.Operator, value: Int) -> NSPredicate

Returns a predicate that checks a category sample’s value.

Deprecated

protocol HKCategoryValuePredicateProviding

A protocol for objects that produce predicates that match category value samples.

### Creating clinical record predicates

class func predicateForClinicalRecords(from: HKSource, fhirResourceType: HKFHIRResourceType, identifier: String) -> NSPredicate

Returns a predicate for a specific FHIR resource.

class func predicateForClinicalRecords(withFHIRResourceType: HKFHIRResourceType) -> NSPredicate

Returns a predicate for a specific FHIR type.

class func predicateForVerifiableClinicalRecords(withRelevantDateWithin: DateInterval) -> NSPredicate

Returns a predicate that finds verifiable health records with a relevant date within the specified range.

### Creating workout predicates

class func predicateForObjects(from: HKWorkout) -> NSPredicate

Returns a predicate that matches any objects that have been associated with the provided workout.

class func predicateForWorkouts(with: HKWorkoutActivityType) -> NSPredicate

Returns a predicate for matching workouts based on the type of activity.

class func predicateForWorkouts(activityPredicate: NSPredicate) -> NSPredicate

Returns a predicate for matching workouts based on the associated workout activities.

class func predicateForWorkouts(with: NSComparisonPredicate.Operator, duration: TimeInterval) -> NSPredicate

Returns a predicate for matching workouts based on their duration.

class func predicateForWorkouts(operatorType: NSComparisonPredicate.Operator, quantityType: HKQuantityType, averageQuantity: HKQuantity) -> NSPredicate

Returns a predicate for matching workouts based the average value of an associated quantity type.

class func predicateForWorkouts(operatorType: NSComparisonPredicate.Operator, quantityType: HKQuantityType, maximumQuantity: HKQuantity) -> NSPredicate

Returns a predicate for matching workout activities based the maximum value of an associated quantity type.

class func predicateForWorkouts(operatorType: NSComparisonPredicate.Operator, quantityType: HKQuantityType, minimumQuantity: HKQuantity) -> NSPredicate

Returns a predicate for matching workout activities based the minimum value of an associated quantity type.

class func predicateForWorkouts(operatorType: NSComparisonPredicate.Operator, quantityType: HKQuantityType, sumQuantity: HKQuantity) -> NSPredicate

Returns a predicate for matching workout activities based the sum of an associated quantity type.

class func predicateForWorkouts(with: NSComparisonPredicate.Operator, totalDistance: HKQuantity) -> NSPredicate

Returns a predicate for matching workouts based on the total distance traveled.

Deprecated

class func predicateForWorkouts(with: NSComparisonPredicate.Operator, totalEnergyBurned: HKQuantity) -> NSPredicate

Returns a predicate for matching workouts based on the total energy burned.

Deprecated

class func predicateForWorkouts(with: NSComparisonPredicate.Operator, totalFlightsClimbed: HKQuantity) -> NSPredicate

Returns a predicate that matches workout samples based on the number of flights climbed.

Deprecated

class func predicateForWorkouts(with: NSComparisonPredicate.Operator, totalSwimmingStrokeCount: HKQuantity) -> NSPredicate

Returns a predicate that matches workout samples based on the number of strokes while swimming.

Deprecated

### Creating workout activity predicates

class func predicateForWorkoutActivities(workoutActivityType: HKWorkoutActivityType) -> NSPredicate

Returns a predicate for workout activities based on the type of activity performed.

class func predicateForWorkoutActivities(operatorType: NSComparisonPredicate.Operator, duration: TimeInterval) -> NSPredicate

Returns a predicate for matching workout activities based on their duration.

class func predicateForWorkoutActivities(start: Date?, end: Date?, options: HKQueryOptions) -> NSPredicate

Returns a predicate for workout activities that occur between the start and end date.

class func predicateForWorkoutActivities(operatorType: NSComparisonPredicate.Operator, quantityType: HKQuantityType, averageQuantity: HKQuantity) -> NSPredicate

Returns a predicate for matching workout activities based the average value of an associated quantity type.

class func predicateForWorkoutActivities(operatorType: NSComparisonPredicate.Operator, quantityType: HKQuantityType, maximumQuantity: HKQuantity) -> NSPredicate

Returns a predicate for matching workout activities based the maximum value of an associated quantity type.

class func predicateForWorkoutActivities(operatorType: NSComparisonPredicate.Operator, quantityType: HKQuantityType, minimumQuantity: HKQuantity) -> NSPredicate

Returns a predicate for matching workout activities based the minimum value of an associated quantity type.

class func predicateForWorkoutActivities(operatorType: NSComparisonPredicate.Operator, quantityType: HKQuantityType, sumQuantity: HKQuantity) -> NSPredicate

Returns a predicate for matching workout activities based the sum of an associated quantity type.

### Creating activity summary predicates

class func predicateForActivitySummary(with: DateComponents) -> NSPredicate

Returns a predicate that matches the activity summary for the specified day.

class func predicate(forActivitySummariesBetweenStart: DateComponents, end: DateComponents) -> NSPredicate

Returns a predicate for matching all the activity summaries that fall between the days identified by the start and end date components.

### Creating electrocardiogram predicates

class func predicateForElectrocardiograms(classification: HKElectrocardiogram.Classification) -> NSPredicate

Returns a predicate that matches electrocardiogram samples with the specified classification.

class func predicateForElectrocardiograms(symptomsStatus: HKElectrocardiogram.SymptomsStatus) -> NSPredicate

Returns a predicate that matches electrocardiogram samples with the specified symptom status.

class func predicateForObjectsAssociated(electrocardiogram: HKElectrocardiogram) -> NSPredicate

Returns a predicate that matches symptom samples associated with the specified electrocardiogram.

### Creating predicate format strings

Use these keys when creating a predicate format string.

Predicate format strings

Formatting strings for creating predicates.

### Creating sort descriptors

HealthKit sort descriptors

Identifiers for sorting results.

### Type Methods

class func predicateForStatesOfMind(with: HKStateOfMind.Label) -> NSPredicate

class func predicateForStatesOfMind(with: HKStateOfMind.Kind) -> NSPredicate

class func predicateForStatesOfMind(with: HKStateOfMind.Association) -> NSPredicate

class func predicateForStatesOfMind(withValence: Double, operatorType: NSComparisonPredicate.Operator) -> NSPredicate

class func predicateForWorkoutEffortSamplesRelated(workout: HKWorkout, activity: HKWorkoutActivity?) -> NSPredicate

## Relationships

### Inherits From

- NSObject

### Inherited By

- HKActivitySummaryQuery
- HKAnchoredObjectQuery
- HKCorrelationQuery
- HKDocumentQuery
- HKElectrocardiogramQuery
- HKHeartbeatSeriesQuery
- HKObserverQuery
- HKQuantitySeriesSampleQuery
- HKSampleQuery
- HKSourceQuery
- HKStatisticsCollectionQuery
- HKStatisticsQuery
- HKVerifiableClinicalRecordQuery
- HKWorkoutEffortRelationshipQuery
- HKWorkoutRouteQuery

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Related Documentation

class HKActivitySummaryQuery

A query for reading activity summary objects from the HealthKit store.

class HKAnchoredObjectQuery

A query that returns changes to the HealthKit store, including a snapshot of new changes and continuous monitoring as a long-running query.

class HKDocumentQuery

A query that returns a snapshot of all matching documents currently saved in the HealthKit store.

class HKObserverQuery

A long-running query that monitors the HealthKit store and updates your app when the HealthKit store saves or deletes a matching sample.

class HKSourceQuery

A query that returns a list of sources, such as apps and devices, that have saved matching queries to the HealthKit store.

class HKStatisticsQuery

A query that performs statistical calculations over a set of matching quantity samples, and returns the results.

class HKStatisticsCollectionQuery

A query that performs multiple statistics queries over a series of fixed-length time intervals.

class HKWorkoutRouteQuery

A query to access the location data stored in a workout route.

### Basic queries

struct HKSampleQueryDescriptor

A query interface that reads samples using Swift concurrency.

class HKSampleQuery

A general query that returns a snapshot of all the matching samples currently saved in the HealthKit store.

class HKCorrelationQuery

A query that performs complex searches based on the correlation’s contents, and returns a snapshot of all matching samples.

class HKQueryDescriptor

A descriptor that specifies a set of samples based on the data type and a predicate.

