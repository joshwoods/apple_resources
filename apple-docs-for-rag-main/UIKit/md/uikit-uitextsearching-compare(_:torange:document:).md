

- UIKit
- UITextSearching
-  compare(\_:toRange:document:) 

Instance Method

# compare(\_:toRange:document:)

Compares ranges from the set of matches the aggregator provides to determine navigation order.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
func compare(
    _ foundRange: UITextRange,
    toRange: UITextRange,
    document: Self.DocumentIdentifier?
) -> ComparisonResult
```

**Required**

## Parameters 

`foundRange`  

The range of characters in a text container to compare from.

`toRange`  

The range of characters in a text container to compare to.

`document`  

A string that uniquely identifies the document containing the text ranges. `Nil` when searching a single document.

## Return Value

Returns the result of comparing the two text ranges.

## Discussion

The system calls this method during a find session to determine which UITextRange to highlight next when a user taps the “next” or “previous” button.

## See Also

### Handling searches

func performTextSearch(queryString: String, options: UITextSearchOptions, resultAggregator: UITextSearchAggregator&lt;Self.DocumentIdentifier>)

Searches for ranges of text matching the string across all searchable documents and collects results in the aggregator.

**Required**

struct UITextSearchAggregator

The methods you use on a find session’s aggregator to collect matching text ranges for a search.

func compare(document: Self.DocumentIdentifier, toDocument: Self.DocumentIdentifier) -> ComparisonResult

Compares documents containing matching ranges from the set the aggregator provides to determine navigation order.

**Required** Default implementation provided.

associatedtype DocumentIdentifier : Hashable = AnyHashable?

An object that uniquely identifies a specific document when searching for matching text across multiple documents.

**Required**

