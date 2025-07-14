

- HealthKit
- HKQuery
-  predicateForWorkouts(with:totalSwimmingStrokeCount:) Deprecated

Type Method

# predicateForWorkouts(with:totalSwimmingStrokeCount:)

Returns a predicate that matches workout samples based on the number of strokes while swimming.

iOS 10.0–18.0DeprecatediPadOS 10.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 3.0–11.0Deprecated

``` source
class func predicateForWorkouts(
    with operatorType: NSComparisonPredicate.Operator,
    totalSwimmingStrokeCount: HKQuantity
) -> NSPredicate
```

Deprecated

Use predicateForWorkoutsWithOperatorType:quantityType:sumQuantity: passing the HKQuantityType for HKQuantityTypeIdentifierSwimmingStrokeCount

## Parameters 

`operatorType`  

The operator to use when comparing the sample to the target number of flights climbed.

`totalSwimmingStrokeCount`  

A quantity representing the target stroke count.

## Return Value

A predicate that matches workouts based on the number of strokes while swimming.

## Discussion

This convenience method creates a predicate that compares the number of swimming strokes during a workout with a target number. The following sample uses the convenience method and a predicate format string to create equivalent predicates.

```
// Creating a predicate using the convenience method.
let swimmingStrokeCount = HKQuantity(unit: HKUnit.count(), doubleValue: 500.0)
let longSwim = HKQuery.predicateForWorkouts(with: .greaterThanOrEqualTo, totalSwimmingStrokeCount: swimmingStrokeCount)

// Creating a predicate using a predicate format string.
let explicitLongSwim = NSPredicate(format: "%K >= %@",
                                   HKPredicateKeyPathWorkoutTotalSwimmingStrokeCount,
                                   swimmingStrokeCount)
```

## See Also

### Related Documentation

let HKPredicateKeyPathWorkoutTotalSwimmingStrokeCount: String

The key path for accessing the number of strokes during a swimming workout.

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

class func predicateForWorkouts(with: NSComparisonPredicate.Operator, totalEnergyBurned: HKQuantity) -> NSPredicate

Returns a predicate for matching workouts based on the total energy burned.

Deprecated

class func predicateForWorkouts(with: NSComparisonPredicate.Operator, totalFlightsClimbed: HKQuantity) -> NSPredicate

Returns a predicate that matches workout samples based on the number of flights climbed.

Deprecated

