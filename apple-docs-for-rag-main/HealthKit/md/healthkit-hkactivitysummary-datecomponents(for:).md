

- HealthKit
- HKActivitySummary
-  dateComponents(for:) 

Instance Method

# dateComponents(for:)

Date components that uniquely identify the day represented by the summary object.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.2+

``` source
func dateComponents(for calendar: Calendar) -> DateComponents
```

## Parameters 

`calendar`  

The calendar used to calculate the date components.

## Return Value

Date components that uniquely specify a day. For example, for the Gregorian calendar, the date components consist of only the era, year, month, and day.

## Discussion

Each activity summary covers a single day. The day always begins and ends at midnight; however, the day may be longer or shorter than 24 hours (for example, if the user traveled across time zones).

## See Also

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

var appleExerciseTimeGoal: HKQuantity

The user’s daily exercise goal.

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

