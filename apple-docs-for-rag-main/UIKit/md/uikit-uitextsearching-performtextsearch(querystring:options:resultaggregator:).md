

- UIKit
- UITextSearching
-  performTextSearch(queryString:options:resultAggregator:) 

Instance Method

# performTextSearch(queryString:options:resultAggregator:)

Searches for ranges of text matching the string across all searchable documents and collects results in the aggregator.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
func performTextSearch(
    queryString: String,
    options: UITextSearchOptions,
    resultAggregator: UITextSearchAggregator
)
```

**Required**

## Parameters 

`queryString`  

The string to search for.

`options`  

The configurable options to use for matching words and comparing strings.

`resultAggregator`  

An object you use to collect matching results. The aggregator is thread-safe, so you may send it messages on other threads.

## Discussion

The system calls this method during a find session to perform the search. Your implenentation should search for matching text ranges in your app’s documents and call foundRange(_:searchString:document:) on the aggregator object to add them to the set of matching ranges.

## See Also

### Handling searches

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

