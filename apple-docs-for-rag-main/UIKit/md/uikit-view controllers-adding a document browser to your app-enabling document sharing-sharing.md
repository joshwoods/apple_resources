

- UIKit
- View controllers
- Adding a document browser to your app
-  Enabling document sharing 

Article

# Enabling document sharing

Give users the ability to import and export documents from your app.

## Overview

The document browser automatically exports the user’s documents when they tap the Share button or perform a drag-and-drop action.

To import documents, your app must specify all the document types that it supports. You typically specify supported document types when you set up your document browser. For additional information, see Set the supported document types.

### Open a shared document

If the user selects your app from the activity view, the system launches your app and calls your app delegate’s application(_:open:options:) method. Implement this method to call your document browser’s revealDocument(at:importIfNeeded:completion:)method to reveal and import the document, as shown in this example:

```
func application(_ app: UIApplication, open inputURL: URL, options: [UIApplicationOpenURLOptionsKey : Any] = [:]) -> Bool {

    // Reveal and import the document at the URL.
    guard let documentBrowserViewController = window?.rootViewController as? DocumentBrowserViewController else {
        fatalError("The root view is not a document browser!")
    }

    documentBrowserViewController.revealDocument(at: inputURL, importIfNeeded: true) { (revealedDocumentURL, error) in

        guard error == nil else {
            os_log("Failed to reveal the document at %@. Error: %@",
                   log: OSLog.default,
                   type: .error,
                   inputURL as CVarArg,
                   error! as CVarArg)
            return
        }

        guard let url = revealedDocumentURL else {
            os_log("No URL revealed",
                   log: OSLog.default,
                   type: .error)

            return
        }

        // You can do something
        // with the revealed document here.
        os_log("Revealed URL: %@",
               log: OSLog.default,
               type: .debug,
               url.path)

        // Present the Document View Controller for the revealed URL.
        documentBrowserViewController.presentDocument(at: revealedDocumentURL!)
    }

    return true
}    
```

If the import is successful, the system calls your document browser delegate’s documentBrowser(_:didImportDocumentAt:toDestinationURL:) method.

## See Also

### Configuration

Setting up a document browser app

Add a document browser view controller to your app.

Presenting selected documents

Display user-selected documents over your browser view controller.

