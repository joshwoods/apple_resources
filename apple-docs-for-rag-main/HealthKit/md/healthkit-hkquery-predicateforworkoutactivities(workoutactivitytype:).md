

- HealthKit
- HKQuery
-  predicateForWorkoutActivities(workoutActivityType:) 

Type Method

# predicateForWorkoutActivities(workoutActivityType:)

Returns a predicate for workout activities based on the type of activity performed.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
class func predicateForWorkoutActivities(workoutActivityType: HKWorkoutActivityType) -> NSPredicate
```

## Parameters 

`workoutActivityType`  

The type of activity. For a list of valid workout activities, see HKWorkoutActivityType.

## Mentioned in 

Dividing a HealthKit workout into activities

## Discussion

To use this predicate, call predicateForWorkouts(activityPredicate:) to wrap this predicate inside a workout predicate. You can then use the workout predicate in your query.

The following example creates a predicate that matches workout activities with a HKWorkoutActivityType.running type.

```
let runningActivityPredicate =
HKQuery.predicateForWorkoutActivities(workoutActivityType: .running)

let workoutPredicate =
HKQuery.predicateForWorkouts(activityPredicate: runningActivityPredicate)
```

## See Also

### Creating workout activity predicates

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

