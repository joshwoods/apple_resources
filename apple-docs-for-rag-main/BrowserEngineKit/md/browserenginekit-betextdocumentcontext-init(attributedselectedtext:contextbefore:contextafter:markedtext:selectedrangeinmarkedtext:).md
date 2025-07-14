

- BrowserEngineKit
- BETextDocumentContext
-  init(attributedSelectedText:contextBefore:contextAfter:markedText:selectedRangeInMarkedText:) 

Initializer

# init(attributedSelectedText:contextBefore:contextAfter:markedText:selectedRangeInMarkedText:)

Initializes a new document context with attributed strings. The `selectedText`, `contextBefore`, and `contextAfter` represent the same ranges as they do in the `-initWithSelectedText:contextBefore:contextAfter:` initializer.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
init(
    attributedSelectedText selectedText: NSAttributedString?,
    contextBefore: NSAttributedString?,
    contextAfter: NSAttributedString?,
    markedText: NSAttributedString?,
    selectedRangeInMarkedText: NSRange
)
```

## See Also

### Creating a text document context

init(selectedText: String?, contextBefore: String?, contextAfter: String?, markedText: String?, selectedRangeInMarkedText: NSRange)

