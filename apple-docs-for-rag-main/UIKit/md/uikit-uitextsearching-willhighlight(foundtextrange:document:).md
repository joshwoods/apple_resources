

- UIKit
- UITextSearching
-  willHighlight(foundTextRange:document:) 

Instance Method

# willHighlight(foundTextRange:document:)

Informs the searchable object when the highlighted search result is about to change.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
func willHighlight(
    foundTextRange: UITextRange,
    document: Self.DocumentIdentifier?
)
```

**Required** Default implementation provided.

## Parameters 

`foundTextRange`  

The text range to highlight.

`document`  

A string that uniquely identifies the document containing the text range. `Nil` when searching a single document.

## Default Implementations

### UITextSearching Implementations

func willHighlight(foundTextRange: UITextRange, document: Self.DocumentIdentifier?)

## See Also

### Displaying results

func decorate(foundTextRange: UITextRange, document: Self.DocumentIdentifier?, usingStyle: UITextSearchFoundTextStyle)

Applies the style to a specific text range to indicate found and highlighted results.

**Required**

func clearAllDecoratedFoundText()

Clears the style from all found and highlighted results.

**Required**

func scrollRangeToVisible(UITextRange, inDocument: Self.DocumentIdentifier?)

Scrolls to the containing view to make the text range visible.

**Required** Default implementation provided.

