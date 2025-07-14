

- SwiftUI
- SearchSuggestionsPlacement
-  SearchSuggestionsPlacement.Set 

Structure

# SearchSuggestionsPlacement.Set

An efficient set of search suggestion display modes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Set
```

## Topics

### Getting placement sets

static var content: SearchSuggestionsPlacement.Set

A set containing placements with the apps main content, excluding the menu placement.

static var menu: SearchSuggestionsPlacement.Set

A set containing the menu display mode.

### Creating a set

init(rawValue: Int)

Creates a set of search suggestions from an integer.

var rawValue: Int

The raw value that records the search suggestion display modes.

### Supporting types

typealias Element

A type for the elements of the set.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

