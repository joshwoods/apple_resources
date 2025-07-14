

- HealthKit
- HKQuery
-  predicateForWorkouts(with:totalEnergyBurned:) Deprecated

Type Method

# predicateForWorkouts(with:totalEnergyBurned:)

Returns a predicate for matching workouts based on the total energy burned.

iOS 8.0–18.0DeprecatediPadOS 8.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 2.0–11.0Deprecated

``` source
class func predicateForWorkouts(
    with operatorType: NSComparisonPredicate.Operator,
    totalEnergyBurned: HKQuantity
) -> NSPredicate
```

Deprecated

Use predicateForWorkoutsWithOperatorType:quantityType:sumQuantity: passing the HKQuantityType for HKQuantityTypeIdentifierActiveEnergyBurned

## Parameters 

`operatorType`  

The operator type to use when comparing the total energy burned.

`totalEnergyBurned`  

The target amount of energy burned.

## Return Value

A predicate for matching workouts based on the total energy burned. This predicate works only on workouts.

## Discussion

Use this convenience method to create a predicate that matches against a workout’s total energy burned. The following sample uses both the convenience method and a predicate format string to create equivalent predicates.

- Swift
- Objective-C

```
// Predicate matching workouts burning 500 calories or more
let energyBurned = HKQuantity(unit: HKUnit.kilocalorieUnit(), doubleValue: 500)
let workout = HKQuery.predicateForWorkoutsWithOperatorType(
    .GreaterThanOrEqualToPredicateOperatorType,
    totalEnergyBurned: energyBurned)

let explicitWorkout = NSPredicate(format: "%K >= %@",
                                  HKPredicateKeyPathWorkoutTotalEnergyBurned, energyBurned)
```

```
// Predicate matching workouts burning 500 calories or more
HKQuantity *energyBurned =
[HKQuantity quantityWithUnit:[HKUnit kilocalorieUnit] doubleValue:500];

NSPredicate *workout =
    [HKQuery predicateForWorkoutsWithOperatorType:
     NSGreaterThanOrEqualToPredicateOperatorType
     totalEnergyBurned:energyBurned];

NSPredicate *explicitWorkout =
[NSPredicate predicateWithFormat:@"%K >= %@",
 HKPredicateKeyPathWorkoutTotalEnergyBurned,
 energyBurned];
```

## See Also

### Related Documentation

let HKPredicateKeyPathWorkoutTotalEnergyBurned: String

The key path for accessing the workout’s total energy burned.

Deprecated

var totalEnergyBurned: HKQuantity?

The total active energy burned during the workout.

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

class func predicateForWorkouts(with: NSComparisonPredicate.Operator, totalDistance: HKQuantity) -> NSPredicate

Returns a predicate for matching workouts based on the total distance traveled.

Deprecated

class func predicateForWorkouts(with: NSComparisonPredicate.Operator, totalFlightsClimbed: HKQuantity) -> NSPredicate

Returns a predicate that matches workout samples based on the number of flights climbed.

Deprecated

class func predicateForWorkouts(with: NSComparisonPredicate.Operator, totalSwimmingStrokeCount: HKQuantity) -> NSPredicate

Returns a predicate that matches workout samples based on the number of strokes while swimming.

Deprecated

