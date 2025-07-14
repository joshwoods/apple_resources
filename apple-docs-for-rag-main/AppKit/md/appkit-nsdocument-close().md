

- AppKit
- NSDocument
-  close() 

Instance Method

# close()

Closes all of the document’s windows and removes the document from its document controller.

macOS

``` source
@MainActor
func close()
```

## Discussion

This method closes the document immediately, without asking users if they want to save the document. This method may not always be called.

## See Also

### Related Documentation

func shouldCloseWindowController(NSWindowController, delegate: Any?, shouldClose: Selector?, contextInfo: UnsafeMutableRawPointer?)

Determines whether the system should close the document and its associated window.

### Closing the Document

func canClose(withDelegate: Any, shouldClose: Selector?, contextInfo: UnsafeMutableRawPointer?)

Determines whether to close the document, prompting the user as needed to choose a course of action.

