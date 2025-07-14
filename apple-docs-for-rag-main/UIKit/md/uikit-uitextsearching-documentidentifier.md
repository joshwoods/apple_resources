

- UIKit
- UITextSearching
-  DocumentIdentifier 

Associated Type

# DocumentIdentifier

An object that uniquely identifies a specific document when searching for matching text across multiple documents.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
associatedtype DocumentIdentifier : Hashable = AnyHashable?
```

**Required**

## Discussion

The UITextSearching and UITextSearchAggregator protocols use this type to distinguish matches in a specific document from text in other documents with the same range.

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

func compare(document: Self.DocumentIdentifier, toDocument: Self.DocumentIdentifier) -> ComparisonResult

Compares documents containing matching ranges from the set the aggregator provides to determine navigation order.

**Required** Default implementation provided.

