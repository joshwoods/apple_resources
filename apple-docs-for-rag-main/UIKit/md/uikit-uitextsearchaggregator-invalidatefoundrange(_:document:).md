

- UIKit
- UITextSearchAggregator
-  invalidateFoundRange(\_:document:) 

Instance Method

# invalidateFoundRange(\_:document:)

Removes a text range from the set of matches.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
func invalidateFoundRange(
    _ range: UITextRange,
    document: DocumentIdentifier
)
```

## Parameters 

`range`  

The text range to remove from the set of matches.

`document`  

A string that uniquely identifies the document containing the text range. `Nil` when searching a single document.

## Discussion

Call this method to invalidate a text range when removing or changing text in the document. This causes the system find panel to update it’s current state, and if the range is the highlighted range, the find panel advances to the next found result.

## See Also

### Tracking search results

func foundRange(UITextRange, searchString: String, document: DocumentIdentifier)

Adds a text range to the set of matches.

func invalidate()

Invalidates all currently shown ranges.

func finishedSearching()

Finishes the search for text ranges.

var allFoundRanges: [UITextRange]

An ordered set of all the text ranges that match the search.

