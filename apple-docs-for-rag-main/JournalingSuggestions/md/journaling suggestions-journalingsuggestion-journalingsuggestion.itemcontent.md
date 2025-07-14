

- Journaling Suggestions
- JournalingSuggestion
-  JournalingSuggestion.ItemContent 

Structure

# JournalingSuggestion.ItemContent

A container for the information about a specific suggestion.

iOS 17.2+

``` source
struct ItemContent
```

## Mentioned in 

Presenting the suggestions picker and processing a selection

## Overview

When a person selects an event in the JournalingSuggestionsPicker, the system invokes the `onCompletion` handler that your app declares for the picker and passes in a JournalingSuggestion instance. The journaling suggestion contains an array of structures of this type in its items property. Each instance of this structure contains one or more concrete instances of JournalingSuggestionAsset that represent the selection in the picker.

## Topics

### Identifying item contents

var id: UUID

The stable identity of the entity associated with this instance.

var representations: [any JournalingSuggestionAsset.Type]

An array of content types that a particular suggestion includes.

### Accessing suggestion data by type

func content&lt;Content>(forType: Content.Type) async throws -> Content?

Retrieves a suggestion’s contents by returning a structure specific to the given content type.

func hasContent&lt;Content>(ofType: Content.Type) -> Bool

Checks if the suggestion contains information for the given type.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Conforms To

- Identifiable

## See Also

### Accessing suggestion data by type

let items: [JournalingSuggestion.ItemContent]

The individual items that compose the suggestion’s content.

func content&lt;Content>(forType: Content.Type) async -> [Content]

Searches a suggestion’s items for information of the given type.

