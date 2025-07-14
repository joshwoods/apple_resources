

- HealthKit
- HKQuery
-  predicateForWorkoutActivities(operatorType:duration:) 

Type Method

# predicateForWorkoutActivities(operatorType:duration:)

Returns a predicate for matching workout activities based on their duration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
class func predicateForWorkoutActivities(
    operatorType: NSComparisonPredicate.Operator,
    duration: TimeInterval
) -> NSPredicate
```

## Parameters 

`operatorType`  

The operator type to use when comparing the duration.

`duration`  

The target duration.

## Return Value

A predicate for matching workout activities based on their duration. This predicate works only on workout activities.

## Discussion

Use this convenience method to create a predicate that matches against an activity’s duration. To use this predicate, call predicateForWorkouts(activityPredicate:) to wrap this predicate inside a workout predicate. You can then use the workout predicate in your query.

The following sample creates a predicate for matching workout activities with a duration of 30 minutes or longer.

```
let longWorkoutActivityPredicate = HKQuery.predicateForWorkoutActivities(operatorType: .greaterThanOrEqualTo, duration: 60.0 * 30.0)

// Wrap the activity predicate inside a workout predicate.
let workoutPredicate = HKQuery.predicateForWorkouts(activityPredicate: longWorkoutActivityPredicate)
```

## See Also

### Related Documentation

let HKPredicateKeyPathWorkoutDuration: String

The key path for accessing the workout’s duration.

var duration: TimeInterval

The workout’s duration.

### Creating workout activity predicates

class func predicateForWorkoutActivities(workoutActivityType: HKWorkoutActivityType) -> NSPredicate

Returns a predicate for workout activities based on the type of activity performed.

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

