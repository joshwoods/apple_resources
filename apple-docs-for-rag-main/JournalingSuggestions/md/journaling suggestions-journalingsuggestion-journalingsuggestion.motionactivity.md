

- Journaling Suggestions
- JournalingSuggestion
-  JournalingSuggestion.MotionActivity 

Structure

# JournalingSuggestion.MotionActivity

A suggestion that describes motion activity, including the number of steps a person takes.

iOS 17.2+

``` source
struct MotionActivity
```

## Mentioned in 

Presenting the suggestions picker and processing a selection

## Overview

The system provides an instance of this structure to your app when a person chooses a motion suggestion in the JournalingSuggestionsPicker.

## Topics

### Accessing motion summary information

var icon: URL?

The URL to an image on disk that depicts the motion activity.

var date: DateInterval?

The range of time in which the motion activity takes place.

### Inspecting motion details

var steps: Int

The number of steps a person takes.

struct MovementType

The movement activity type that the phone records when it detects motion.

var movementType: JournalingSuggestion.MotionActivity.MovementType?

The specific type of movement associated with the activity.

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

struct WorkoutGroup

A suggestion that contains multiple workouts that a person chooses in the picker.

