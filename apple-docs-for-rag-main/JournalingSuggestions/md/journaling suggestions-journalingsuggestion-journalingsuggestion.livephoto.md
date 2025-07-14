

- Journaling Suggestions
- JournalingSuggestion
-  JournalingSuggestion.LivePhoto 

Structure

# JournalingSuggestion.LivePhoto

A suggestion for a Live Photo from a person’s library.

iOS 17.2+

``` source
struct LivePhoto
```

## Mentioned in 

Presenting the suggestions picker and processing a selection

## Overview

The system provides an instance of this structure to your app when a person chooses a Live Photo suggestion in the JournalingSuggestionsPicker.

## Topics

### Accessing Live Photo data

var image: URL

The URL to a still image on disk for the Live Photo.

var video: URL

The URL to a video on disk for the Live Photo..

var date: Date?

The Live Photo’s creation date.

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

struct WorkoutGroup

A suggestion that contains multiple workouts that a person chooses in the picker.

