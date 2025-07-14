

- UIKit
- UITextSearching
-  scrollRangeToVisible(\_:inDocument:) 

Instance Method

# scrollRangeToVisible(\_:inDocument:)

Scrolls to the containing view to make the text range visible.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
func scrollRangeToVisible(
    _ range: UITextRange,
    inDocument: Self.DocumentIdentifier?
)
```

**Required** Default implementation provided.

## Parameters 

`range`  

The text range to scroll to.

`inDocument`  

A string that uniquely identifies the document containing the text range. `Nil` when searching a single document.

## Discussion

If the seachable object supports scrolling, use this method to implement scrolling your view to make the highlighted text range visible.

## Default Implementations

### UITextSearching Implementations

func scrollRangeToVisible(UITextRange, inDocument: Self.DocumentIdentifier?)

## See Also

### Displaying results

func decorate(foundTextRange: UITextRange, document: Self.DocumentIdentifier?, usingStyle: UITextSearchFoundTextStyle)

Applies the style to a specific text range to indicate found and highlighted results.

**Required**

func clearAllDecoratedFoundText()

Clears the style from all found and highlighted results.

**Required**

func willHighlight(foundTextRange: UITextRange, document: Self.DocumentIdentifier?)

Informs the searchable object when the highlighted search result is about to change.

**Required** Default implementation provided.

