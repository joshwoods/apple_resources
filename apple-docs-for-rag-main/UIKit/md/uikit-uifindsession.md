

- UIKit
-  UIFindSession 

Class

# UIFindSession

An abstract base class that manages the state, presentation, and behavior for a search that the find interaction initiates.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
class UIFindSession
```

## Overview

You return a session object from the delegate of a UIFindInteraction to manage the state, presentation, and behavior for a given search. The session object responds to navigation and replacement requests through its highlightNextResult(in:) and performSingleReplacement(query:replacementString:options:) methods. It also provides presentation information to the system find panel through resultCount and highlightedResultIndex.

UIKit can manage the state when you implement the UITextSearching protocol on a class that encapsulates the searchable content. To do this, create an instance of UITextSearchingFindSession and provide it a searchableObject using an instance of your class.

If you want to manage the state yourself or already have a class that implements find and replace for your app, you can subclass UIFindSession to bridge your custom implementation to the system UI.

## Topics

### Getting session information

var resultCount: Int

The total number of results the search matches.

var highlightedResultIndex: Int

The index of the result the find panel highlights.

var supportsReplacement: Bool

A Boolean value that indicates whether to allow replacing find panel results.

var allowsReplacementForCurrentlyHighlightedResult: Bool

A Boolean value that indicates whether to allow replacing the result the find panel is highlighting.

var searchResultDisplayStyle: UIFindSession.SearchResultDisplayStyle

The information the find panel includes in the summary of found results.

enum SearchResultDisplayStyle

Constants that describe the results summary the find panel UI includes.

### Managing session interactions

func performSearch(query: String, options: UITextSearchOptions?)

Initiates a search for the query string you provide.

func performSingleReplacement(query: String, replacementString: String, options: UITextSearchOptions?)

Replaces a single instance of the query string with the replacement string you provide.

func replaceAll(searchQuery: String, replacementString: String, options: UITextSearchOptions?)

Replaces all matching instances of the query string with the replacement string you provide.

func highlightNextResult(in: UITextStorageDirection)

Updates the highlighted result to the next or previous match.

func invalidateFoundResults()

Invalidates the found ranges and updates the system find panel.

### Deprecated

var allowsReplacement: Bool

A Boolean value that indicates whether to allow replacing the result the find panel is highlighting.

Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- UITextSearchingFindSession

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Find and replace

class UIFindInteraction

An interaction that provides text finding and replacing operations using a system find panel.

protocol UIFindInteractionDelegate

A delegate object that provides a session object to manage the search state for a find interaction and receives notifications of search session lifetimes.

class UITextSearchingFindSession

A find session object that wraps a searchable object implementing the text-searching protocol.

protocol UITextSearching

The methods you use on a find session’s searchable objects to perform search operations and decorate the found text results.

class UITextSearchOptions

An object containing the configurable options for a text search.

enum UITextSearchFoundTextStyle

Constants that describe the style a find session uses to decorate the text.

enum WordMatchMethod

Constants that describe the method to use when searching text for words that match a string.

enum SearchResultDisplayStyle

Constants that describe the results summary the find panel UI includes.

