

- UIKit
- UITextSearching
-  decorate(foundTextRange:document:usingStyle:) 

Instance Method

# decorate(foundTextRange:document:usingStyle:)

Applies the style to a specific text range to indicate found and highlighted results.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
func decorate(
    foundTextRange: UITextRange,
    document: Self.DocumentIdentifier?,
    usingStyle: UITextSearchFoundTextStyle
)
```

**Required**

## Parameters 

`foundTextRange`  

The text range to decorate.

`document`  

A string that uniquely identifies the document containing the text range. `Nil` when searching a single document.

`usingStyle`  

The style to decorate the text: highlighted, found, or normal.

## Discussion

The system calls this method during a find session to display the results of a search in your custom view. Your implenentation should decorate matching text ranges for the given style to indicate the found and highlighted result.

## See Also

### Displaying results

func clearAllDecoratedFoundText()

Clears the style from all found and highlighted results.

**Required**

func willHighlight(foundTextRange: UITextRange, document: Self.DocumentIdentifier?)

Informs the searchable object when the highlighted search result is about to change.

**Required** Default implementation provided.

func scrollRangeToVisible(UITextRange, inDocument: Self.DocumentIdentifier?)

Scrolls to the containing view to make the text range visible.

**Required** Default implementation provided.

