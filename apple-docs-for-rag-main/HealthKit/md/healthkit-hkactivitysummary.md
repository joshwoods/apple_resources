

- HealthKit
-  HKActivitySummary 

Class

# HKActivitySummary

An object that contains the move, exercise, and stand data for a given day.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.2+

``` source
class HKActivitySummary
```

## Mentioned in 

Executing Activity Summary Queries

## Overview

You can read HKActivitySummary objects from the HealthKit store using an HKActivitySummaryQuery object. Unlike the HKSample subclasses, HKActivitySummary instances are mutable, but changes made to the object’s properties have no affect on the values in the HealthKit store.

You can instantiate your own HKActivitySummary objects (if needed), but you can’t save HKActivitySummary objects to the store.

You can display an active summary in iOS using the HKActivityRingView class or in watchOS using the WKInterfaceActivityRing class.

## Topics

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

func dateComponents(for: Calendar) -> DateComponents

Date components that uniquely identify the day represented by the summary object.

### Specifying predicate key paths

let HKPredicateKeyPathDateComponents: String

The key path for accessing an activity summary’s date components.

### Instance Properties

var isPaused: Bool

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Activity rings

struct HKActivitySummaryQueryDescriptor

A query interface that reads activity summaries using Swift concurrency.

class HKActivitySummaryQuery

A query for reading activity summary objects from the HealthKit store.

class HKActivityRingView

A view that uses the Move, Exercise, and Stand activity rings to display data from a HealthKit activity summary object.

class HKActivityMoveModeObject

An object that contains a movement mode value.

