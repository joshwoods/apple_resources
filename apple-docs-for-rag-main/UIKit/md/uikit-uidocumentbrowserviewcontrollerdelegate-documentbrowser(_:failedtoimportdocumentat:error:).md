

- UIKit
- UIDocumentBrowserViewControllerDelegate
-  documentBrowser(\_:failedToImportDocumentAt:error:) 

Instance Method

# documentBrowser(\_:failedToImportDocumentAt:error:)

Tells the delegate that the document browser failed to import the specified document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentBrowser(
    _ controller: UIDocumentBrowserViewController,
    failedToImportDocumentAt documentURL: URL,
    error: (any Error)?
)
```

## Parameters 

`controller`  

The document browser that attempted the import action.

`documentURL`  

The document’s original URL.

`error`  

An object describing the error, or `nil`.

## See Also

### Creating new documents

func documentBrowser(UIDocumentBrowserViewController, didRequestDocumentCreationWithHandler: (URL?, UIDocumentBrowserViewController.ImportMode) -> Void)

Asks the delegate to create a new document.

enum ImportMode

The document browser’s import modes.

func documentBrowser(UIDocumentBrowserViewController, didImportDocumentAt: URL, toDestinationURL: URL)

Tells the delegate that a document has been successfully imported.

