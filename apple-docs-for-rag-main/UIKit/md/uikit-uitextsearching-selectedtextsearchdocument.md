

- UIKit
- UITextSearching
-  selectedTextSearchDocument 

Instance Property

# selectedTextSearchDocument

The object that uniquely identifies the specific document with selected text.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
var selectedTextSearchDocument: Self.DocumentIdentifier? { get }
```

**Required** Default implementation provided.

## Discussion

When performing a search across multiple documents, this object returns the identifier for the document with the selected text. When performing a search on a single document, it returns `nil`.

## Default Implementations

### UITextSearching Implementations

var selectedTextSearchDocument: Self.DocumentIdentifier?

## See Also

### Identifying selected text

var selectedTextRange: UITextRange?

The range of selected text in a document.

**Required**

