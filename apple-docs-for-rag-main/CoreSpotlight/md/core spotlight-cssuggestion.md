

- Core Spotlight
-  CSSuggestion 

Class

# CSSuggestion

The kind of suggestion to use in a query.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class CSSuggestion
```

## Mentioned in 

Building a search interface for your app

## Overview

Your app uses `CSSuggestion` objects to populate a contextual menu of suggestions.

## Topics

### Setting suggestion attributes

var localizedAttributedSuggestion: AttributedString

An attributed string for the localized suggestion.

var suggestionKind: CSSuggestion.SuggestionKind

The type of suggestion.

enum SuggestionKind

The suggestion type that determines how the system handles a suggestion.

### Comparing suggestions

func compare(CSSuggestion) -> ComparisonResult

Compares the suggestion with a second specified suggestion.

func compare(byRank: CSSuggestion) -> ComparisonResult

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Queries

Building a search interface for your app

Add a search interface to your app to execute Spotlight queries and offer suggested text completions.

Searching for information in your app

Search for app-specific content and refine search results using predicates and filters.

class CSUserQuery

A type you use to initiate searches from your interface and offer suggested text completions.

class CSUserQueryContext

The configuration details to apply to a user query.

class CSSearchQuery

A type you use to programmatically search the indexed app content.

class CSSearchQueryContext

The behavior configuration to use for a search query.

