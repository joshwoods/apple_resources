

- HealthKit
- Queries
- HKQuery
-  Predicate format strings 

API Collection

# Predicate format strings

Formatting strings for creating predicates.

## Topics

### Object keys

let HKPredicateKeyPathUUID: String

The key path for accessing the object’s UUID inside a predicate format string.

let HKPredicateKeyPathMetadata: String

The key path for accessing the object’s metadata dictionary inside a predicate format string.

let HKPredicateKeyPathSum: String

The key path for accessing the sum of a quantity series inside a predicate format string.

### Quantity sample keys

let HKPredicateKeyPathQuantity: String

The key path for accessing the sample’s quantity.

### Category sample keys

let HKPredicateKeyPathCategoryValue: String

The key path for accessing the category sample’s value.

### Correlation sample keys

let HKPredicateKeyPathCorrelation: String

The key path for accessing the object’s correlation inside a predicate format string.

### Device and source keys

let HKPredicateKeyPathDevice: String

The key path for accessing the object’s device inside a predicate format string.

let HKPredicateKeyPathSource: String

The key path for accessing the object’s source inside a predicate format string.

let HKPredicateKeyPathSourceRevision: String

The key path for accessing the object’s source revision inside a predicate format string.

### Start and end date keys

let HKPredicateKeyPathStartDate: String

The key path for accessing the sample’s start date.

let HKPredicateKeyPathEndDate: String

The key path for accessing the sample’s end date.

### Activity summary keys

let HKPredicateKeyPathDateComponents: String

The key path for accessing an activity summary’s date components.

### Document keys

let HKPredicateKeyPathCDAAuthorName: String

The key path for accessing the author’s name inside a predicate format string.

let HKPredicateKeyPathCDACustodianName: String

The key path for accessing the custodian’s name inside a predicate format string.

let HKPredicateKeyPathCDAPatientName: String

The key path for accessing the patient’s name inside a predicate format string.

let HKPredicateKeyPathCDATitle: String

The key path for accessing the document’s title inside a predicate format string.

### Clinical record keys

let HKPredicateKeyPathClinicalRecordFHIRResourceIdentifier: String

The key path for accessing the clinical record’s Fast Healthcare Interoperability Resources (FHIR) identifier.

let HKPredicateKeyPathClinicalRecordFHIRResourceType: String

The key path for accessing the resource type of a Fast Healthcare Interoperability Resources (FHIR) record.

### Workout keys

let HKPredicateKeyPathWorkout: String

The key path for accessing the object’s workout inside a predicate format string.

let HKPredicateKeyPathWorkoutType: String

The key path for accessing the workout’s type.

let HKPredicateKeyPathWorkoutDuration: String

The key path for accessing the workout’s duration.

let HKPredicateKeyPathWorkoutAverageQuantity: String

The key path for accessing workouts with a matching average quantity.

let HKPredicateKeyPathWorkoutMaximumQuantity: String

The key path for accessing workouts with a matching maximum quantity.

let HKPredicateKeyPathWorkoutMinimumQuantity: String

The key path for accessing workouts with a matching minimum quantity.

let HKPredicateKeyPathWorkoutSumQuantity: String

The key path for accessing workouts with a matching sum.

let HKPredicateKeyPathWorkoutTotalDistance: String

The key path for accessing the workout’s total distance.

Deprecated

let HKPredicateKeyPathWorkoutTotalEnergyBurned: String

The key path for accessing the workout’s total energy burned.

Deprecated

let HKPredicateKeyPathWorkoutTotalFlightsClimbed: String

The key path for accessing the total number of flights of stairs climbed during the workout.

Deprecated

let HKPredicateKeyPathWorkoutTotalSwimmingStrokeCount: String

The key path for accessing the number of strokes during a swimming workout.

Deprecated

### Workout activity keys

let HKPredicateKeyPathWorkoutActivity: String

The key path for accessing a specific workout activity.

let HKPredicateKeyPathWorkoutActivityType: String

The key path for accessing activities that match a workout activity type.

let HKPredicateKeyPathWorkoutActivityStartDate: String

The key path for accessing activities with a matching start date.

let HKPredicateKeyPathWorkoutActivityEndDate: String

The key path for accessing activities with a matching end date.

let HKPredicateKeyPathWorkoutActivityDuration: String

The key path for accessing activities with a matching duration.

let HKPredicateKeyPathWorkoutActivityAverageQuantity: String

The key path for accessing activities with a matching average quantity.

let HKPredicateKeyPathWorkoutActivityMaximumQuantity: String

The key path for accessing activities with a matching maximum quantity.

let HKPredicateKeyPathWorkoutActivityMinimumQuantity: String

The key path for accessing activities with a matching minimum quantity.

let HKPredicateKeyPathWorkoutActivitySumQuantity: String

The key path for accessing activities with a matching sum.

