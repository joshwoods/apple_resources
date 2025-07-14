

- UIKit
-  UISearchSuggestionItem 

Class

# UISearchSuggestionItem

A selectable search parameter.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
class UISearchSuggestionItem
```

## Overview

This class provides a basic implementation of the UISearchSuggestion protocol.

## Topics

### Creating a search suggestion

init(localizedSuggestion: String, localizedDescription: String?, iconImage: UIImage?)

Creates a search suggestion with the specified text and image attributes.

init(localizedAttributedSuggestion: NSAttributedString, localizedDescription: String?, iconImage: UIImage?)

Creates a search suggestion with the specified attributed label, accessibility description, and image.

init(localizedSuggestion: String, localizedDescription: String?)

Creates a search suggestion with the specified label and accessibility description.

init(localizedAttributedSuggestion: NSAttributedString, localizedDescription: String?)

Creates a search suggestion with the specified attributed label and accessibility description.

init(localizedSuggestion: String)

Creates a search suggestion with the specified label.

init(localizedAttributedSuggestion: NSAttributedString)

Creates a search suggestion with the specified attributed label.

### Describing a search suggestion

var localizedSuggestion: String?

A label for the suggestion, usually the search term the suggestion represents.

var localizedAttributedSuggestion: NSAttributedString?

An attributed label for the suggestion, usually the search term the suggestion represents.

var localizedDescription: String?

A description of the suggestion.

var iconImage: UIImage?

An image for display on the suggestion.

var representedObject: Any?

An object for tracking supplementary information about the search suggestion.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UISearchSuggestion

## See Also

### Providing search suggestions

var searchSuggestions: [any UISearchSuggestion]?

A list of suggestions to offer as shortcuts below the search field.

var ignoresSearchSuggestionsForSearchBarPlacementStacked: Bool

A Boolean value you use to specify whether the search controller prevents search suggestions from displaying for a stacked search bar.

protocol UISearchSuggestion

A set of attributes that a selectable search suggestion must provide.

