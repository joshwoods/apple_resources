

- Journaling Suggestions
- JournalingSuggestion
-  JournalingSuggestion.GenericMedia 

Structure

# JournalingSuggestion.GenericMedia

A suggestion describing now playable media that a person listened to.

iOS 18.0+

``` source
struct GenericMedia
```

## Mentioned in 

Presenting the suggestions picker and processing a selection

## Overview

The system provides an instance of this structure to your app when a person chooses a media suggestion in the JournalingSuggestionsPicker. To exclude the Now Playing item from content suggestions, refer to mpnowplayinginfopropertyexcludefromsuggestions.

## Topics

### Accessing media data

var album: String?

The name of the album that contains the media item.

var appIcon: URL?

The URL to an image on disk for the Now Playing app that played the media item.

var artist: String?

The performing artists for a media item.

var date: Date?

The media item’s playback date.

var title: String?

The title or name of a media item.

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

