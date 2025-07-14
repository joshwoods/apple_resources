

- HealthKit
-  HKActivityMoveMode 

Enumeration

# HKActivityMoveMode

Constants that specify the value measured by the Move ring on the user’s device.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
enum HKActivityMoveMode
```

## Overview

For younger users, HealthKit’s activity summary can track move time instead of active energy burned:

- HealthKit encourages users under 13 years old to track move time.

- Users 13 to 18 years old can choose to track move time or active energy burned.

- All users over 18 years old track active energy burned.

## Topics

### Move Modes

case activeEnergy

A value that indicates the Move ring measures active energy burned.

case appleMoveTime

A value that indicates the Activity app’s Move ring measures Apple Move Time.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing the summary’s data

var activityMoveMode: HKActivityMoveMode

The move mode that they system used for this activity summary.

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

func dateComponents(for: Calendar) -> DateComponents

Date components that uniquely identify the day represented by the summary object.

