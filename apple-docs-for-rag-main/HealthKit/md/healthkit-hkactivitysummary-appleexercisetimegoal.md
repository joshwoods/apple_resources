

- HealthKit
- HKActivitySummary
-  appleExerciseTimeGoal 

Instance Property

# appleExerciseTimeGoal

The user’s daily exercise goal.

iOS 9.3–18.4DeprecatediPadOS 9.3–18.4DeprecatedMac Catalyst 13.1+macOS 13.0+visionOS 1.0–2.4DeprecatedwatchOS 2.2–11.4Deprecated

``` source
var appleExerciseTimeGoal: HKQuantity { get set }
```

## Discussion

The HKQuantity object for this property must use time units.

## See Also

### Related Documentation

static let appleExerciseTime: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of time the user spent exercising.

### Accessing the summary’s data

var activityMoveMode: HKActivityMoveMode

The move mode that they system used for this activity summary.

enum HKActivityMoveMode

Constants that specify the value measured by the Move ring on the user’s device.

var activeEnergyBurned: HKQuantity

The amount of active energy the user burned during the specified day.

var activeEnergyBurnedGoal: HKQuantity

The user’s daily goal for active energy burned.

var appleMoveTime: HKQuantity

The amount of time the user spent performing activities that involve full-body movements during the specified day.

var appleMoveTimeGoal: HKQuantity

The user’s daily goal for move time.

var appleExerciseTime: HKQuantity

The amount of time that the user has spent exercising during the specified day.

var exerciseTimeGoal: HKQuantity?

The user’s daily goal for exercise time.

var appleStandHours: HKQuantity

The number hours in the specified day during which the user has stood and moved for at least a minute per hour.

var standHoursGoal: HKQuantity?

The user’s daily goal for stand hours.

var appleStandHoursGoal: HKQuantity

The user’s daily goal for stand hours.

enum HKCategoryValueAppleStandHour

Categories that the system used to indicate whether the user stood during the sample’s duration.

func dateComponents(for: Calendar) -> DateComponents

Date components that uniquely identify the day represented by the summary object.

