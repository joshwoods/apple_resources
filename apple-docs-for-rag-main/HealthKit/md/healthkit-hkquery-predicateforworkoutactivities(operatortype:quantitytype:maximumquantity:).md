

- HealthKit
- HKQuery
-  predicateForWorkoutActivities(operatorType:quantityType:maximumQuantity:) 

Type Method

# predicateForWorkoutActivities(operatorType:quantityType:maximumQuantity:)

Returns a predicate for matching workout activities based the maximum value of an associated quantity type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
class func predicateForWorkoutActivities(
    operatorType: NSComparisonPredicate.Operator,
    quantityType: HKQuantityType,
    maximumQuantity: HKQuantity
) -> NSPredicate
```

## Parameters 

`operatorType`  

The operator type to use when comparing the maximum quantity.

`quantityType`  

The type of HKQuantitySample objects used to calculate the maximum quantity.

`maximumQuantity`  

The target value for the maximum quantity.

## Discussion

Use this convenience method to create a predicate that matches workout activities with the specified maximum quantity. To use this predicate, call predicateForWorkouts(activityPredicate:) to wrap this predicate inside a workout predicate. You can then use the workout predicate in your query.

The following sample creates a predicate for workout activities with a maximum heart rate of 150 bmp or higher.

```
let quantityType = HKQuantityType(.heartRate)

let expectedQuantity =
HKQuantity(unit: .count().unitDivided(by: .minute()),
           doubleValue: 150.0)

let heartRatePredicate =
HKQuery.predicateForWorkoutActivities(
    operatorType: .greaterThanOrEqualTo,
    quantityType: quantityType,
    maximumQuantity:
        expectedQuantity
)

// Wrap the activity predicate inside a workout predicate.
let workoutPredicate = HKQuery.predicateForWorkouts(activityPredicate: heartRatePredicate)
```

For more information on how HealthKit calculates statistics for HKWorkoutActivity objects, see statistics(for:).

## See Also

### Creating workout activity predicates

class func predicateForWorkoutActivities(workoutActivityType: HKWorkoutActivityType) -> NSPredicate

Returns a predicate for workout activities based on the type of activity performed.

class func predicateForWorkoutActivities(operatorType: NSComparisonPredicate.Operator, duration: TimeInterval) -> NSPredicate

Returns a predicate for matching workout activities based on their duration.

class func predicateForWorkoutActivities(start: Date?, end: Date?, options: HKQueryOptions) -> NSPredicate

Returns a predicate for workout activities that occur between the start and end date.

class func predicateForWorkoutActivities(operatorType: NSComparisonPredicate.Operator, quantityType: HKQuantityType, averageQuantity: HKQuantity) -> NSPredicate

Returns a predicate for matching workout activities based the average value of an associated quantity type.

class func predicateForWorkoutActivities(operatorType: NSComparisonPredicate.Operator, quantityType: HKQuantityType, minimumQuantity: HKQuantity) -> NSPredicate

Returns a predicate for matching workout activities based the minimum value of an associated quantity type.

class func predicateForWorkoutActivities(operatorType: NSComparisonPredicate.Operator, quantityType: HKQuantityType, sumQuantity: HKQuantity) -> NSPredicate

Returns a predicate for matching workout activities based the sum of an associated quantity type.

