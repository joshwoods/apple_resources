

- UIKit
- UITextSearchAggregator
-  finishedSearching() 

Instance Method

# finishedSearching()

Finishes the search for text ranges.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
func finishedSearching()
```

## Discussion

Call this method after searching all documents.

## See Also

### Tracking search results

func foundRange(UITextRange, searchString: String, document: DocumentIdentifier)

Adds a text range to the set of matches.

func invalidateFoundRange(UITextRange, document: DocumentIdentifier)

Removes a text range from the set of matches.

func invalidate()

Invalidates all currently shown ranges.

var allFoundRanges: [UITextRange]

An ordered set of all the text ranges that match the search.

