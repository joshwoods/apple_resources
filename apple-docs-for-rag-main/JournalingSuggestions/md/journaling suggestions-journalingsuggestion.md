

- Journaling Suggestions
-  JournalingSuggestion 

Structure

# JournalingSuggestion

High-level information about a suggestion that a person chooses in the journaling suggestions picker.

iOS 17.2+

``` source
struct JournalingSuggestion
```

## Overview

When a person chooses a particular suggestion in the JournalingSuggestionsPicker, the system provides your app with more information about the event by passing an instance of this structure to your picker’s `onCompletion` handler.

## Topics

### Inspecting suggestion details

let date: DateInterval?

The range of time in which the suggested event takes place.

let title: String

The title for the suggestion.

### Accessing suggestion data by type

let items: [JournalingSuggestion.ItemContent]

The individual items that compose the suggestion’s content.

struct ItemContent

A container for the information about a specific suggestion.

func content&lt;Content>(forType: Content.Type) async -> [Content]

Searches a suggestion’s items for information of the given type.

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

struct WorkoutGroup

A suggestion that contains multiple workouts that a person chooses in the picker.

### Instance Properties

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Implementation

struct JournalingSuggestionsPicker

A view that lists different types of recent events in a person’s life.

protocol JournalingSuggestionAsset

An interface for the content that the suggestions picker presents.

