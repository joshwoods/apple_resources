

- Journaling Suggestions
-  JournalingSuggestionsPicker 

Structure

# JournalingSuggestionsPicker

A view that lists different types of recent events in a person’s life.

iOS 17.2+

``` source
@MainActor @preconcurrency
struct JournalingSuggestionsPicker where Label : View
```

## Mentioned in 

Presenting the suggestions picker and processing a selection

## Overview

This interface displays several grids of content that layout visual mementos, each representing unique, personal events that occur in a person’s life. It enables a person to reflect and choose a particular event as a topic for derivative work. For example, a workout can serve as the beginnings of a new journal entry or illustration.

The first time the picker appears, a modal sheet introduces the concept of journaling suggestions. After a person selects a suggestion in the picker, the system shares only the information associated with the chosen suggestion with your app.

For more information, see Presenting the suggestions picker and processing a selection.

## Topics

### Creating a suggestions picker

init(label: () -> Label, onCompletion: (JournalingSuggestion) async -> Void)

Creates a suggestions picker within the given view.

init(LocalizedStringKey, onCompletion: (JournalingSuggestion) async -> Void)

Creates a suggestions picker with button text defined by the given localized string key.

init&lt;S>(S, onCompletion: (JournalingSuggestion) async -> Void)

Creates a suggestions picker with button text defined by the given string.

### Displaying a suggestions picker

var body: some View

The content and behavior of the view.

### Type Aliases

typealias Body

The type of view representing the body of this view.

### Default Implementations

View Implementations

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Implementation

struct JournalingSuggestion

High-level information about a suggestion that a person chooses in the journaling suggestions picker.

protocol JournalingSuggestionAsset

An interface for the content that the suggestions picker presents.

