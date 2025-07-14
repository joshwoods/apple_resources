

- UIKit
- UITextSearchAggregator
-  foundRange(\_:searchString:document:) 

Instance Method

# foundRange(\_:searchString:document:)

Adds a text range to the set of matches.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
func foundRange(
    _ range: UITextRange,
    searchString: String,
    document: DocumentIdentifier
)
```

## Parameters 

`range`  

The text range to add to the set of matches.

`searchString`  

The query string the search used to locate this range of text.

`document`  

A string that uniquely identifies the document containing the text range. `Nil` when searching a single document.

## Discussion

Call this method to add a text range found in your document to the set of matches.

## See Also

### Tracking search results

func invalidateFoundRange(UITextRange, document: DocumentIdentifier)

Removes a text range from the set of matches.

func invalidate()

Invalidates all currently shown ranges.

func finishedSearching()

Finishes the search for text ranges.

var allFoundRanges: [UITextRange]

An ordered set of all the text ranges that match the search.

