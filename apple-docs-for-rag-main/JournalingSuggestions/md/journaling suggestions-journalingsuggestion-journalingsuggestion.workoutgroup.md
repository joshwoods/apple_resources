

- Journaling Suggestions
- JournalingSuggestion
-  JournalingSuggestion.WorkoutGroup 

Structure

# JournalingSuggestion.WorkoutGroup

A suggestion that contains multiple workouts that a person chooses in the picker.

iOS 17.2+

``` source
struct WorkoutGroup
```

## Overview

The system provides an instance of this structure to your app when a person chooses multiple workout suggestions in the JournalingSuggestionsPicker.

## Topics

### Accessing workout summary information

var icon: URL?

The URL to an image on disc that represents the types of completed workout.

var duration: TimeInterval?

The amount of time the workouts span.

var activeEnergyBurned: HKQuantity?

The total energy that the person burns over the workouts.

var averageHeartRate: HKQuantity?

The average heart rate that the person experiences during the workouts.

### Accessing individual workouts

var workouts: [JournalingSuggestion.Workout]

An array of workout suggestions that a person chooses in the picker.

### Type Aliases

typealias JournalingSuggestionContent

Represents a generic content type for journaling suggestions.

## Relationships

### Conforms To

- JournalingSuggestionAsset

## See Also

### Interacting with suggestion types

struct Contact

A suggestion for a connection a person makes with someone else.

struct GenericMedia

A suggestion describing now playable media that a person listened to.

struct LivePhoto

A suggestion for a Live Photo from a person’s library.

struct Location

A suggestion that represents a location that a person visits.

struct LocationGroup

A suggestion that contains multiple visited locations that a person chooses in the picker.

struct MotionActivity

A suggestion that describes motion activity, including the number of steps a person takes.

struct Photo

A suggestion for a photo from a person’s library.

struct Podcast

A suggestion that describes a podcast episode a person listened to.

struct Reflection

A suggestion for a reflection prompt.

struct StateOfMind

A suggestion that describes a state of mind reflection in the Health app.

struct Song

A suggestion for a song from a person’s music library.

struct Video

A suggestion for a video from a person’s library.

struct Workout

A suggestion that describes a workout that a person completed.

