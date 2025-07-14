

- HealthKit
- HKQuery
-  predicateForWorkouts(with:duration:) 

Type Method

# predicateForWorkouts(with:duration:)

Returns a predicate for matching workouts based on their duration.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func predicateForWorkouts(
    with operatorType: NSComparisonPredicate.Operator,
    duration: TimeInterval
) -> NSPredicate
```

## Parameters 

`operatorType`  

The operator type to use when comparing the duration.

`duration`  

The target duration.

## Return Value

A predicate for matching workouts based on their duration. This predicate works only on workouts.

## Discussion

Use this convenience method to create a predicate that matches against a workout’s duration. The following sample uses both the convenience method and a predicate format string to create equivalent predicates.

- Swift
- Objective-C

```
// Predicate matching workouts equal to or longer than 30 minutes
let workout = HKQuery.predicateForWorkoutsWithOperatorType(
    .GreaterThanOrEqualToPredicateOperatorType,
    duration: 60.0 * 30.0)

let explicitWorkout = NSPredicate(format: "%K >= %d",
                                  HKPredicateKeyPathWorkoutDuration, 60 * 30)
```

```
// Predicate matching workouts equal to or longer than 30 minutes
NSPredicate *workout =
    [HKQuery predicateForWorkoutsWithOperatorType:

     NSGreaterThanOrEqualToPredicateOperatorType
      duration:60.0 * 30.0];

NSPredicate *explicitWorkout =
[NSPredicate predicateWithFormat:@"%K >= %d",
 HKPredicateKeyPathWorkoutDuration,
 60 * 30];
```

## See Also

### Related Documentation

let HKPredicateKeyPathWorkoutDuration: String

The key path for accessing the workout’s duration.

var duration: TimeInterval

The workout’s duration.

### Creating workout predicates

class func predicateForObjects(from: HKWorkout) -> NSPredicate

Returns a predicate that matches any objects that have been associated with the provided workout.

class func predicateForWorkouts(with: HKWorkoutActivityType) -> NSPredicate

Returns a predicate for matching workouts based on the type of activity.

class func predicateForWorkouts(activityPredicate: NSPredicate) -> NSPredicate

Returns a predicate for matching workouts based on the associated workout activities.

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

