

- UIKit
- UITextSearching
-  compare(document:toDocument:) 

Instance Method

# compare(document:toDocument:)

Compares documents containing matching ranges from the set the aggregator provides to determine navigation order.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
func compare(
    document: Self.DocumentIdentifier,
    toDocument: Self.DocumentIdentifier
) -> ComparisonResult
```

**Required** Default implementation provided.

## Parameters 

`document`  

A string that uniquely identifies the document to compare from.

`toDocument`  

A string that uniquely identifies the document to compare to.

## Return Value

Returns the result of comparing the two documents.

## Discussion

The system calls this method during a find session to determine which document’s ranges to highlight next when a user taps the “next” or “previous” button. Return ComparisonResult.orderedAscending if the text ranges found in the `fromDocument` come before those found in the `toDocument` in your view. Otherwise, return ComparisonResult.orderedDescending.

The system only calls this method if you provide document identifiers to the session’s result aggregator.

## Default Implementations

### UITextSearching Implementations

func compare(document: Self.DocumentIdentifier, toDocument: Self.DocumentIdentifier) -> ComparisonResult

## See Also

### Handling searches

func performTextSearch(queryString: String, options: UITextSearchOptions, resultAggregator: UITextSearchAggregator&lt;Self.DocumentIdentifier>)

Searches for ranges of text matching the string across all searchable documents and collects results in the aggregator.

**Required**

struct UITextSearchAggregator

The methods you use on a find session’s aggregator to collect matching text ranges for a search.

func compare(UITextRange, toRange: UITextRange, document: Self.DocumentIdentifier?) -> ComparisonResult

Compares ranges from the set of matches the aggregator provides to determine navigation order.

**Required**

associatedtype DocumentIdentifier : Hashable = AnyHashable?

An object that uniquely identifies a specific document when searching for matching text across multiple documents.

**Required**

