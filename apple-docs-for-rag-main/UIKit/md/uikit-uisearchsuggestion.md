

- UIKit
-  UISearchSuggestion 

Protocol

# UISearchSuggestion

A set of attributes that a selectable search suggestion must provide.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
protocol UISearchSuggestion : NSObjectProtocol
```

## Overview

Provide common or predicted search queries to save the user the time of typing their entire query in a UISearchController field. UISearchSuggestionItem provides a simple implementation of this protocol. You may also define and use your own type that conforms to UISearchSuggestion.

## Topics

### Describing a search suggestion

var localizedSuggestion: String?

A label for the suggestion, usually the search term the suggestion represents.

**Required**

var localizedDescription: String?

A description of the suggestion.

var localizedAttributedSuggestion: NSAttributedString?

An attributed label for the suggestion, usually the search term the suggestion represents.

**Required**

var iconImage: UIImage?

An image for display on the suggestion.

var representedObject: Any?

An object for tracking supplementary information about the search suggestion.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UISearchSuggestionItem

## See Also

### Providing search suggestions

var searchSuggestions: [any UISearchSuggestion]?

A list of suggestions to offer as shortcuts below the search field.

var ignoresSearchSuggestionsForSearchBarPlacementStacked: Bool

A Boolean value you use to specify whether the search controller prevents search suggestions from displaying for a stacked search bar.

class UISearchSuggestionItem

A selectable search parameter.

