

- UIKit
- UITextSearching
-  clearAllDecoratedFoundText() 

Instance Method

# clearAllDecoratedFoundText()

Clears the style from all found and highlighted results.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
func clearAllDecoratedFoundText()
```

**Required**

## See Also

### Displaying results

func decorate(foundTextRange: UITextRange, document: Self.DocumentIdentifier?, usingStyle: UITextSearchFoundTextStyle)

Applies the style to a specific text range to indicate found and highlighted results.

**Required**

func willHighlight(foundTextRange: UITextRange, document: Self.DocumentIdentifier?)

Informs the searchable object when the highlighted search result is about to change.

**Required** Default implementation provided.

func scrollRangeToVisible(UITextRange, inDocument: Self.DocumentIdentifier?)

Scrolls to the containing view to make the text range visible.

**Required** Default implementation provided.

