

- HealthKit
- HKQuery
-  predicateForWorkouts(with:totalFlightsClimbed:) Deprecated

Type Method

# predicateForWorkouts(with:totalFlightsClimbed:)

Returns a predicate that matches workout samples based on the number of flights climbed.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 4.0–11.0Deprecated

``` source
class func predicateForWorkouts(
    with operatorType: NSComparisonPredicate.Operator,
    totalFlightsClimbed: HKQuantity
) -> NSPredicate
```

Deprecated

Use predicateForWorkoutsWithOperatorType:quantityType:sumQuantity: passing the HKQuantityType for HKQuantityTypeIdentifierFlightsClimbed

## Parameters 

`operatorType`  

The operator to use when comparing the sample to the target number of flights climbed.

`totalFlightsClimbed`  

A quantity representing the target number of flights climbed.

## Return Value

A predicate that matches workouts based on the number of flights climbed.

## Discussion

This convenience method creates a predicate that compares the total flights climbed during a workout with a target number of flights climbed. The following sample uses the convenience method and a predicate format string to create equivalent predicates.

```
let flightsClimbed = HKQuantity(unit: HKUnit.count(), doubleValue: 10.0)
let tenFlightsClimbed = HKQuery.predicateForWorkouts(with: .greaterThanOrEqualTo, totalFlightsClimbed: flightsClimbed)

// Creating a predicate using a predicate format string.
let explicitTenFlightsClimbed = NSPredicate(format: "%K >= %@",
                                            HKPredicateKeyPathWorkoutTotalFlightsClimbed,
                                            flightsClimbed)
```

## See Also

### Related Documentation

let HKPredicateKeyPathWorkoutTotalFlightsClimbed: String

The key path for accessing the total number of flights of stairs climbed during the workout.

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

class func predicateForWorkouts(with: NSComparisonPredicate.Operator, totalSwimmingStrokeCount: HKQuantity) -> NSPredicate

Returns a predicate that matches workout samples based on the number of strokes while swimming.

Deprecated

