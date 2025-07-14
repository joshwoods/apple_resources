

- HealthKit
- HKQuery
-  predicateForWorkouts(with:) 

Type Method

# predicateForWorkouts(with:)

Returns a predicate for matching workouts based on the type of activity.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func predicateForWorkouts(with workoutActivityType: HKWorkoutActivityType) -> NSPredicate
```

## Parameters 

`workoutActivityType`  

The type of activity. For a list of valid workout activities, see HKWorkoutActivityType.

## Return Value

A predicate for matching workouts based on the type of activity.

## Discussion

Use this convenience method to create a predicate that matches workouts based on their activity. The following sample uses both the convenience method and a predicate format string to create equivalent predicates.

- Swift
- Objective-C

```
let workout = HKQuery.predicateForWorkoutsWithWorkoutActivityType(.Curling)

let explicitWorkout = NSPredicate(format: "%K == %d",
                                  HKPredicateKeyPathWorkoutType,
                                  HKWorkoutActivityType.Curling.rawValue)
```

```
NSPredicate *workout =
    [HKQuery predicateForWorkoutsWithWorkoutActivityType:
     HKWorkoutActivityTypeCurling];

NSPredicate *explicitWorkout =
[NSPredicate predicateWithFormat:@"%K == %d",
 HKPredicateKeyPathWorkoutType,
 HKWorkoutActivityTypeCurling];
```

## See Also

### Related Documentation

var workoutActivityType: HKWorkoutActivityType

The type of activity performed during the workout.

let HKPredicateKeyPathWorkoutType: String

The key path for accessing the workout’s type.

### Creating workout predicates

class func predicateForObjects(from: HKWorkout) -> NSPredicate

Returns a predicate that matches any objects that have been associated with the provided workout.

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

