

- HealthKit
- HKQuery
-  predicateForWorkouts(operatorType:quantityType:sumQuantity:) 

Type Method

# predicateForWorkouts(operatorType:quantityType:sumQuantity:)

Returns a predicate for matching workout activities based the sum of an associated quantity type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
class func predicateForWorkouts(
    operatorType: NSComparisonPredicate.Operator,
    quantityType: HKQuantityType,
    sumQuantity: HKQuantity
) -> NSPredicate
```

## Parameters 

`operatorType`  

The operator type to use when comparing the sum.

`quantityType`  

The type of HKQuantitySample objects used to calculate the sum.

`sumQuantity`  

The target value for the sum.

## Discussion

Use this convenience method to create a predicate that matches workouts with the specified total value. For more information on how HealthKit calculates statistics for HKWorkoutActivity objects, see statistics(for:).

The following sample creates a predicate for workout activities with a total step count of 1000 or higher.

```
let quantityType = HKQuantityType(.stepCount)

let expectedQuantity = HKQuantity(unit: .count(),
                                  doubleValue: 1000.0)

let stepCountPredicate = HKQuery.predicateForWorkouts(
    operatorType: .greaterThanOrEqualTo,
    quantityType: quantityType,
    sumQuantity: expectedQuantity)
```

## See Also

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

