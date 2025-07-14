

- UIKit
-  UITextSearching 

Protocol

# UITextSearching

The methods you use on a find session’s searchable objects to perform search operations and decorate the found text results.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
protocol UITextSearching : NSObjectProtocol
```

## Overview

Implement this protocol on the class that encapsulates the searchable content for your view. This allows you to use an instance of UITextSearchingFindSession to manage the session for a find interaction.

## Topics

### Handling searches

func performTextSearch(queryString: String, options: UITextSearchOptions, resultAggregator: UITextSearchAggregator&lt;Self.DocumentIdentifier>)

Searches for ranges of text matching the string across all searchable documents and collects results in the aggregator.

**Required**

struct UITextSearchAggregator

The methods you use on a find session’s aggregator to collect matching text ranges for a search.

func compare(UITextRange, toRange: UITextRange, document: Self.DocumentIdentifier?) -> ComparisonResult

Compares ranges from the set of matches the aggregator provides to determine navigation order.

**Required**

func compare(document: Self.DocumentIdentifier, toDocument: Self.DocumentIdentifier) -> ComparisonResult

Compares documents containing matching ranges from the set the aggregator provides to determine navigation order.

**Required** Default implementation provided.

associatedtype DocumentIdentifier : Hashable = AnyHashable?

An object that uniquely identifies a specific document when searching for matching text across multiple documents.

**Required**

### Displaying results

func decorate(foundTextRange: UITextRange, document: Self.DocumentIdentifier?, usingStyle: UITextSearchFoundTextStyle)

Applies the style to a specific text range to indicate found and highlighted results.

**Required**

func clearAllDecoratedFoundText()

Clears the style from all found and highlighted results.

**Required**

func willHighlight(foundTextRange: UITextRange, document: Self.DocumentIdentifier?)

Informs the searchable object when the highlighted search result is about to change.

**Required** Default implementation provided.

func scrollRangeToVisible(UITextRange, inDocument: Self.DocumentIdentifier?)

Scrolls to the containing view to make the text range visible.

**Required** Default implementation provided.

### Identifying selected text

var selectedTextRange: UITextRange?

The range of selected text in a document.

**Required**

var selectedTextSearchDocument: Self.DocumentIdentifier?

The object that uniquely identifies the specific document with selected text.

**Required** Default implementation provided.

### Handling replacements

var supportsTextReplacement: Bool

A Boolean value that indicates whether the searchable object supports replacing text.

**Required** Default implementation provided.

func replace(foundTextRange: UITextRange, document: Self.DocumentIdentifier?, withText: String)

Informs the searchable object to replace the text range for the highlighted search result.

**Required** Default implementation provided.

func replaceAll(queryString: String, options: UITextSearchOptions, withText: String)

Informs the searchable object to replace all matching text across all searchable documents.

**Required** Default implementation provided.

func shouldReplace(foundTextRange: UITextRange, document: Self.DocumentIdentifier?, withText: String) -> Bool

Determines whether the searchable object allows replacement of the text range you provide.

**Required** Default implementation provided.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UITextView

## See Also

### Find and replace

class UIFindInteraction

An interaction that provides text finding and replacing operations using a system find panel.

protocol UIFindInteractionDelegate

A delegate object that provides a session object to manage the search state for a find interaction and receives notifications of search session lifetimes.

class UIFindSession

An abstract base class that manages the state, presentation, and behavior for a search that the find interaction initiates.

class UITextSearchingFindSession

A find session object that wraps a searchable object implementing the text-searching protocol.

class UITextSearchOptions

An object containing the configurable options for a text search.

enum UITextSearchFoundTextStyle

Constants that describe the style a find session uses to decorate the text.

enum WordMatchMethod

Constants that describe the method to use when searching text for words that match a string.

enum SearchResultDisplayStyle

Constants that describe the results summary the find panel UI includes.

