

- HealthKit
- HKQuery
-  predicateForObjects(from:) 

Type Method

# predicateForObjects(from:)

Returns a predicate that matches any objects that have been associated with the provided workout.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func predicateForObjects(from workout: HKWorkout) -> NSPredicate
```

## Parameters 

`workout`  

The workout you are searching for.

## Return Value

A predicate that matches any objects that have been added to the provided workout.

## Mentioned in 

Adding samples to a workout

## Discussion

Use this convenience method to create a predicate that matches all the HealthKit objects for a given workout. The following sample uses both the convenience method and a predicate format string to create equivalent predicates.

- Swift
- Objective-C

```
let workoutObjects = HKQuery.predicateForObjectsFromWorkout(workout)

let explicitWorkoutObjects =
    NSPredicate(format: "%K == %@", HKPredicateKeyPathWorkout, workout)
```

```
NSPredicate *workoutObjects = [HKQuery predicateForObjectsFromWorkout:workout];

NSPredicate *explicitWorkoutObjects =
[NSPredicate predicateWithFormat:@"%K == %@",
 HKPredicateKeyPathWorkout,
 workout];
```

## See Also

### Related Documentation

func add([HKSample], to: HKWorkout, completion: (Bool, (any Error)?) -> Void)

Associates the provided samples with the specified workout.

Deprecated

### Creating workout predicates

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

