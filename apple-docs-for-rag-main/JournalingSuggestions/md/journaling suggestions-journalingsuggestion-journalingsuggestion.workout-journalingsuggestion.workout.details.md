

- Journaling Suggestions
- JournalingSuggestion
- JournalingSuggestion.Workout
-  JournalingSuggestion.Workout.Details 

Structure

# JournalingSuggestion.Workout.Details

Information about a workout that a person completes.

iOS 17.2+

``` source
struct Details
```

## Overview

Each JournalingSuggestion.Workout contains an instance of this structure with its details property.

## Topics

### Instance Properties

var activeEnergyBurned: HKQuantity?

The energy that a person burns during the workout.

var activityType: HKWorkoutActivityType

The type of workout.

var averageHeartRate: HKQuantity?

The average heart rate that a person experiences during the workout.

var date: DateInterval?

The range of time in which the workout takes place.

var distance: HKQuantity?

The distance that the workout spans.

### Type Aliases

typealias JournalingSuggestionContent

Represents a generic content type for journaling suggestions.

## Relationships

### Conforms To

- JournalingSuggestionAsset

## See Also

### Inspecting workout details

var details: JournalingSuggestion.Workout.Details?

A structure that contains the workout specifics.

