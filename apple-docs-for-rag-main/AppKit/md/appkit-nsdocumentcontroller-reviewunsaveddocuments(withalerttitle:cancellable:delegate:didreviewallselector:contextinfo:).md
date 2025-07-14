

- AppKit
- NSDocumentController
-  reviewUnsavedDocuments(withAlertTitle:cancellable:delegate:didReviewAllSelector:contextInfo:) 

Instance Method

# reviewUnsavedDocuments(withAlertTitle:cancellable:delegate:didReviewAllSelector:contextInfo:)

Displays an alert asking if the user wants to review unsaved documents, quit regardless of unsaved documents, or cancel the save operation.

macOS

``` source
@MainActor
func reviewUnsavedDocuments(
    withAlertTitle title: String?,
    cancellable: Bool,
    delegate: Any?,
    didReviewAllSelector: Selector?,
    contextInfo: UnsafeMutableRawPointer?
)
```

## Parameters 

`title`  

The title of the alert.

`cancellable`  

A Boolean indicating whether the operation can be canceled.

`delegate`  

The object that calls the selector.

`didReviewAllSelector`  

The selector to call when all documents have been reviewed.

`contextInfo`  

A pointer to user-supplied data.

## Discussion

Assigns `delegate` to the panel. Calls `didReviewAllSelector` with true if quit without saving is chosen or if there are no dirty documents, and false otherwise. If the user selects the “Review Unsaved” option, closeAllDocuments(withDelegate:didCloseAllSelector:contextInfo:) is called. This method is called when the user chooses the Quit menu command, and also when the computer power is being turned off. Note that `title` is ignored. Pass the `contextInfo` object with the callback.

The `didReviewAllSelector` callback method should have the following signature:

```
- (void)documentController:(NSDocumentController *)docController  didReviewAll: (BOOL)didReviewAll contextInfo:(void *)contextInfo
```

## See Also

### Closing Documents

func closeAllDocuments(withDelegate: Any?, didCloseAllSelector: Selector?, contextInfo: UnsafeMutableRawPointer?)

Iterates through all the open documents and tries to close them one by one using the specified delegate.

