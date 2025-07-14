

- UIKit
-  UITextSearchAggregator 

Structure

# UITextSearchAggregator

The methods you use on a find session’s aggregator to collect matching text ranges for a search.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
struct UITextSearchAggregator where DocumentIdentifier : Hashable
```

## Overview

To track text ranges that match the search, call these methods on the aggregator for the searchable object implementing the UITextSearching protocol for a UITextSearchingFindSession.

## Topics

### Tracking search results

func foundRange(UITextRange, searchString: String, document: DocumentIdentifier)

Adds a text range to the set of matches.

func invalidateFoundRange(UITextRange, document: DocumentIdentifier)

Removes a text range from the set of matches.

func invalidate()

Invalidates all currently shown ranges.

func finishedSearching()

Finishes the search for text ranges.

var allFoundRanges: [UITextRange]

An ordered set of all the text ranges that match the search.

## See Also

### Handling searches

func performTextSearch(queryString: String, options: UITextSearchOptions, resultAggregator: UITextSearchAggregator&lt;Self.DocumentIdentifier>)

Searches for ranges of text matching the string across all searchable documents and collects results in the aggregator.

**Required**

func compare(UITextRange, toRange: UITextRange, document: Self.DocumentIdentifier?) -> ComparisonResult

Compares ranges from the set of matches the aggregator provides to determine navigation order.

**Required**

func compare(document: Self.DocumentIdentifier, toDocument: Self.DocumentIdentifier) -> ComparisonResult

Compares documents containing matching ranges from the set the aggregator provides to determine navigation order.

**Required** Default implementation provided.

associatedtype DocumentIdentifier : Hashable = AnyHashable?

An object that uniquely identifies a specific document when searching for matching text across multiple documents.

**Required**

