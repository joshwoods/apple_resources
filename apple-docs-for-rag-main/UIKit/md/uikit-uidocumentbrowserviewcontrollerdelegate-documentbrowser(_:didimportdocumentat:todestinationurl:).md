

- UIKit
- UIDocumentBrowserViewControllerDelegate
-  documentBrowser(\_:didImportDocumentAt:toDestinationURL:) 

Instance Method

# documentBrowser(\_:didImportDocumentAt:toDestinationURL:)

Tells the delegate that a document has been successfully imported.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentBrowser(
    _ controller: UIDocumentBrowserViewController,
    didImportDocumentAt sourceURL: URL,
    toDestinationURL destinationURL: URL
)
```

## Parameters 

`controller`  

The document browser that performed the import action.

`sourceURL`  

The document’s original URL.

`destinationURL`  

The document’s URL after the import.

## Mentioned in 

Enabling document sharing

## Discussion

To open the document as soon as it’s imported:

1.  Open a new UIDocument subclass for the document (or use a file presenter and file coordination to access the document).

2.  Create a view controller to display the document.

3.  Present that view controller modally.

## See Also

### Creating new documents

func documentBrowser(UIDocumentBrowserViewController, didRequestDocumentCreationWithHandler: (URL?, UIDocumentBrowserViewController.ImportMode) -> Void)

Asks the delegate to create a new document.

enum ImportMode

The document browser’s import modes.

func documentBrowser(UIDocumentBrowserViewController, failedToImportDocumentAt: URL, error: (any Error)?)

Tells the delegate that the document browser failed to import the specified document.

