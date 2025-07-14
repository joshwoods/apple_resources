

- HealthKit
- HKQuery
-  predicateForWorkouts(with:totalDistance:) Deprecated

Type Method

# predicateForWorkouts(with:totalDistance:)

Returns a predicate for matching workouts based on the total distance traveled.

iOS 8.0–18.4DeprecatediPadOS 8.0–18.4DeprecatedMac Catalyst 13.0+macOS 13.0–15.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
class func predicateForWorkouts(
    with operatorType: NSComparisonPredicate.Operator,
    totalDistance: HKQuantity
) -> NSPredicate
```

Deprecated

Use predicateForWorkoutsWithOperatorType:quantityType:sumQuantity: passing the HKQuantityType for the desired distance type

## Parameters 

`operatorType`  

The operator type to use when comparing the total distance.

`totalDistance`  

The target distance.

## Return Value

A predicate for matching workouts based on the total distance traveled. This predicate works only on workouts.

## Discussion

Use this convenience method to create a predicate that matches against a workout’s total distance. The following sample uses both the convenience method and a predicate format string to create equivalent predicates.

- Swift
- Objective-C

```
// Predicate matching workouts covering 6.5 miles or more.
let distance = HKQuantity(unit: HKUnit.mileUnit(), doubleValue: 6.5)
let workout = HKQuery.predicateForWorkoutsWithOperatorType(
    .GreaterThanOrEqualToPredicateOperatorType,
    totalDistance: distance)

let explicitWorkout = NSPredicate(format: "%K >= %@",
                                  HKPredicateKeyPathWorkoutTotalDistance, distance)
```

```
// Predicate matching workouts covering 6.5 miles or more.
HKQuantity *distance =
    [HKQuantity quantityWithUnit:[HKUnit mileUnit] doubleValue:6.5];

NSPredicate *workout =
    [HKQuery predicateForWorkoutsWithOperatorType:
     NSGreaterThanOrEqualToPredicateOperatorType
     totalDistance:distance];

NSPredicate *explicitWorkout =
[NSPredicate predicateWithFormat:@"%K >= %@",
 HKPredicateKeyPathWorkoutTotalDistance,
 distance];
```

## See Also

### Related Documentation

var totalDistance: HKQuantity?

The total distance traveled during the workout.

Deprecated

let HKPredicateKeyPathWorkoutTotalDistance: String

The key path for accessing the workout’s total distance.

Deprecated

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

class func predicateForWorkouts(with: NSComparisonPredicate.Operator, totalEnergyBurned: HKQuantity) -> NSPredicate

Returns a predicate for matching workouts based on the total energy burned.

Deprecated

class func predicateForWorkouts(with: NSComparisonPredicate.Operator, totalFlightsClimbed: HKQuantity) -> NSPredicate

Returns a predicate that matches workout samples based on the number of flights climbed.

Deprecated

class func predicateForWorkouts(with: NSComparisonPredicate.Operator, totalSwimmingStrokeCount: HKQuantity) -> NSPredicate

Returns a predicate that matches workout samples based on the number of strokes while swimming.

Deprecated

