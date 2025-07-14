

- UIKit
- UITextSearchAggregator
-  invalidate() 

Instance Method

# invalidate()

Invalidates all currently shown ranges.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
func invalidate()
```

## Discussion

Calling this method causes the system find panel to update its current state, and might trigger a new search using performTextSearch(queryString:options:resultAggregator:) (Swift) or performTextSearchWithQueryString:usingOptions:resultAggregator: (Objective-C) immediately after.

## See Also

### Tracking search results

func foundRange(UITextRange, searchString: String, document: DocumentIdentifier)

Adds a text range to the set of matches.

func invalidateFoundRange(UITextRange, document: DocumentIdentifier)

Removes a text range from the set of matches.

func finishedSearching()

Finishes the search for text ranges.

var allFoundRanges: [UITextRange]

An ordered set of all the text ranges that match the search.

