

- Journaling Suggestions
- JournalingSuggestion
-  JournalingSuggestion.Workout 

Structure

# JournalingSuggestion.Workout

A suggestion that describes a workout that a person completed.

iOS 17.2+

``` source
struct Workout
```

## Mentioned in 

Presenting the suggestions picker and processing a selection

## Overview

The system provides an instance of this structure to your app when a person chooses a workout suggestion in the JournalingSuggestionsPicker.

## Topics

### Accessing workout summary information

var icon: URL?

The URL to an image on disc that represents the type of workout.

var route: [CLLocation]?

The geographic path that a person travels over the course of the workout.

### Inspecting workout details

var details: JournalingSuggestion.Workout.Details?

A structure that contains the workout specifics.

struct Details

Information about a workout that a person completes.

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

struct WorkoutGroup

A suggestion that contains multiple workouts that a person chooses in the picker.

