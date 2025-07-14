

- AppKit
- NSDocumentController
-  closeAllDocuments(withDelegate:didCloseAllSelector:contextInfo:) 

Instance Method

# closeAllDocuments(withDelegate:didCloseAllSelector:contextInfo:)

Iterates through all the open documents and tries to close them one by one using the specified delegate.

macOS

``` source
@MainActor
func closeAllDocuments(
    withDelegate delegate: Any?,
    didCloseAllSelector: Selector?,
    contextInfo: UnsafeMutableRawPointer?
)
```

## Parameters 

`delegate`  

The object responsible for closing the document.

`didCloseAllSelector`  

The selector to call after all documents have been closed.

`contextInfo`  

A pointer to user-supplied data.

## Discussion

Each `NSDocument` object is sent canClose(withDelegate:shouldClose:contextInfo:), which, if the document is dirty, gives it a chance to refuse to close or to save itself first. This method may ask whether to save or to perform a save.

The `didCloseAllSelector` callback method is called with true if all documents are closed, and false otherwise. Pass the `contextInfo` object with the callback. The `didCloseAllSelector` callback method should have the following signature:

```
- (void)documentController:(NSDocumentController *)docController  didCloseAll:(BOOL)didCloseAll contextInfo:(void *)contextInfo
```

## See Also

### Closing Documents

func reviewUnsavedDocuments(withAlertTitle: String?, cancellable: Bool, delegate: Any?, didReviewAllSelector: Selector?, contextInfo: UnsafeMutableRawPointer?)

Displays an alert asking if the user wants to review unsaved documents, quit regardless of unsaved documents, or cancel the save operation.

