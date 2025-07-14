

- UIKit
- UIDocumentBrowserViewControllerDelegate
-  documentBrowser(\_:didRequestDocumentCreationWithHandler:) 

Instance Method

# documentBrowser(\_:didRequestDocumentCreationWithHandler:)

Asks the delegate to create a new document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentBrowser(
    _ controller: UIDocumentBrowserViewController,
    didRequestDocumentCreationWithHandler importHandler: @escaping (URL?, UIDocumentBrowserViewController.ImportMode) -> Void
)
```

## Parameters 

`controller`  

The current document browser.

`importHandler`  

A block that takes the following parameters:

urlToImport  
The URL of the document’s initial, temporary location.

importMode  
The mode used when importing the document. For a list of import modes, see UIDocumentBrowserViewController.ImportMode.

## Mentioned in 

Customizing the browser

Customizing a document-based app’s launch experience

## Discussion

Implement this method to create new documents for the user:

1.  (Optional) Display any controls the user needs to configure the document.

2.  Create a new document and save it to a temporary location. If you use a UIDocument subclass to create the document, you must close it before calling the `importHandler` block. Always open a new document in your documentBrowser(_:didImportDocumentAt:toDestinationURL:) method.

3.  Call the provided `importHandler` block. To confirm the request, pass in the document’s temporary URL and the import mode (UIDocumentBrowserViewController.ImportMode.copy or UIDocumentBrowserViewController.ImportMode.move). To cancel the request, pass `nil` and UIDocumentBrowserViewController.ImportMode.none.

4.  Implement the documentBrowser(_:didImportDocumentAt:toDestinationURL:) method. In this method, open the document at the destination URL. You must use either a UIDocument subclass, or a file presenter and file coordination.

5.  Modally present this document to the user.

Important

You must always call the import handler. If you cannot create a new document, pass `nil` for the URL and UIDocumentBrowserViewController.ImportMode.none for the import mode.

The following example shows a possible implementation of the documentBrowser(_:didRequestDocumentCreationWithHandler:) method.

```
// Create New Document
func documentBrowser(_ controller: UIDocumentBrowserViewController, didRequestDocumentCreationWithHandler importHandler: @escaping (URL?, UIDocumentBrowserViewController.ImportMode) -> Void) {

    let doc = // Create a new UIDocument... 
    let url = // Get a temporary URL...

    // Create a new document in a temporary location
    doc.save(to: url, for: .forCreating) { (saveSuccess) in

        // Make sure the document saved successfully
        guard saveSuccess else {            
            // Cancel document creation
            importHandler(nil, .none)
            return
        }

        // Close the document.
        doc.close(completionHandler: { (closeSuccess) in

            // Make sure the document closed successfully
            guard closeSuccess else {                
                // Cancel document creation
                importHandler(nil, .none)
                return
            }

            // Pass the document's temporary URL to the import handler.
            importHandler(url, .move)
        })
    }
}
```

After the `importHandler` block is called, the document browser asynchronously imports the document into its final destination. When possible, the document browser imports to the currently open directory. When there is no currently open directory (for example, when the Recents tab is open), it uses the default directory.

Users can set the default directory in Settings. For more information, see Setting up a document browser app.

When the import is complete, the browser calls one of the following delegate methods:

- **On success.** documentBrowser(_:didImportDocumentAt:toDestinationURL:)

- **On failure.** documentBrowser(_:failedToImportDocumentAt:error:)

The document browser enables the Add button (+) only when both of the following are true:

- The allowsDocumentCreation property is set to true (the default value).

- The document browser delegate implements the documentBrowser(_:didRequestDocumentCreationWithHandler:) method.

Note

The document browser cannot create new documents if you do not implement this delegate method.

## See Also

### Creating new documents

enum ImportMode

The document browser’s import modes.

func documentBrowser(UIDocumentBrowserViewController, didImportDocumentAt: URL, toDestinationURL: URL)

Tells the delegate that a document has been successfully imported.

func documentBrowser(UIDocumentBrowserViewController, failedToImportDocumentAt: URL, error: (any Error)?)

Tells the delegate that the document browser failed to import the specified document.

