

- Core Spotlight
- CSSuggestion
-  CSSuggestion.SuggestionKind 

Enumeration

# CSSuggestion.SuggestionKind

The suggestion type that determines how the system handles a suggestion.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
enum SuggestionKind
```

## Overview

Suggestions that the system returns from the query handler have CSSuggestion.SuggestionKind.default.

## Topics

### Suggestion types

case none

Blocks the system from displaying the suggestion.

case custom

Sorts the custom suggestions together.

case `default`

Displays the suggestion normally.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting suggestion attributes

var localizedAttributedSuggestion: AttributedString

An attributed string for the localized suggestion.

var suggestionKind: CSSuggestion.SuggestionKind

The type of suggestion.

