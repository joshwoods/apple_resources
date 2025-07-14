

- Journaling Suggestions
-  JournalingSuggestionAsset 

Protocol

# JournalingSuggestionAsset

An interface for the content that the suggestions picker presents.

iOS 17.2+

``` source
protocol JournalingSuggestionAsset
```

## Mentioned in 

Presenting the suggestions picker and processing a selection

## Overview

When a person makes a selection in a JournalingSuggestionsPicker, the system invokes the picker’s `onCompletion` closure, and passes in the selected suggestion (JournalingSuggestion). Each item in the suggestion’s items array conforms to this protocol.

## Topics

### Associated Types

associatedtype JournalingSuggestionContent : JournalingSuggestionAsset = Self

Represents a generic content type for journaling suggestions.

**Required**

## Relationships

### Conforming Types

- JournalingSuggestion.Contact
- JournalingSuggestion.GenericMedia
- JournalingSuggestion.LivePhoto
- JournalingSuggestion.Location
- JournalingSuggestion.LocationGroup
- JournalingSuggestion.MotionActivity
- JournalingSuggestion.Photo
- JournalingSuggestion.Podcast
- JournalingSuggestion.Reflection
- JournalingSuggestion.Song
- JournalingSuggestion.StateOfMind
- JournalingSuggestion.Video
- JournalingSuggestion.Workout
- JournalingSuggestion.Workout.Details
- JournalingSuggestion.WorkoutGroup

## See Also

### Implementation

struct JournalingSuggestionsPicker

A view that lists different types of recent events in a person’s life.

struct JournalingSuggestion

High-level information about a suggestion that a person chooses in the journaling suggestions picker.

