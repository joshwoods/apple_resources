

- UIKit
- UITextSearching
-  selectedTextRange 

Instance Property

# selectedTextRange

The range of selected text in a document.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
var selectedTextRange: UITextRange? { get }
```

**Required**

## Discussion

If the text range has a length, it indicates the currently selected text. If it has zero length, it indicates the caret (insertion point). If the text-range object is `nil`, it indicates that there’s no current selection.

## See Also

### Identifying selected text

var selectedTextSearchDocument: Self.DocumentIdentifier?

The object that uniquely identifies the specific document with selected text.

**Required** Default implementation provided.

