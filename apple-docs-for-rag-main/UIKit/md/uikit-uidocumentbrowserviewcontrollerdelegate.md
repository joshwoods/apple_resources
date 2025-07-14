

- UIKit
-  UIDocumentBrowserViewControllerDelegate 

Protocol

# UIDocumentBrowserViewControllerDelegate

The protocol you implement to respond as the user interacts with the document browser.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
protocol UIDocumentBrowserViewControllerDelegate : NSObjectProtocol
```

## Mentioned in 

Customizing a document-based app’s launch experience

Adding custom actions and activities

Customizing the browser

## Topics

### Creating new documents

func documentBrowser(UIDocumentBrowserViewController, didRequestDocumentCreationWithHandler: (URL?, UIDocumentBrowserViewController.ImportMode) -> Void)

Asks the delegate to create a new document.

enum ImportMode

The document browser’s import modes.

func documentBrowser(UIDocumentBrowserViewController, didImportDocumentAt: URL, toDestinationURL: URL)

Tells the delegate that a document has been successfully imported.

func documentBrowser(UIDocumentBrowserViewController, failedToImportDocumentAt: URL, error: (any Error)?)

Tells the delegate that the document browser failed to import the specified document.

### Selecting documents

func documentBrowser(UIDocumentBrowserViewController, didPickDocumentsAt: [URL])

Tells the delegate that the user has selected one or more documents.

### Working with the browser’s activity view

func documentBrowser(UIDocumentBrowserViewController, willPresent: UIActivityViewController)

Tells the delegate that the document browser will display an activity view.

func documentBrowser(UIDocumentBrowserViewController, applicationActivitiesForDocumentURLs: [URL]) -> [UIActivity]

Asks the delegate for additional activities when displaying an activity view.

### Deprecated methods

func documentBrowser(UIDocumentBrowserViewController, didPickDocumentURLs: [URL])

Tells the delegate that the user has selected one or more documents.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Related Documentation

class UIDocumentBrowserViewController

A view controller for browsing and performing actions on documents that you store locally and in the cloud.

### Responding to browser events

var delegate: (any UIDocumentBrowserViewControllerDelegate)?

The document browser’s delegate.

func importDocument(at: URL, nextToDocumentAt: URL, mode: UIDocumentBrowserViewController.ImportMode, completionHandler: (URL?, (any Error)?) -> Void)

Imports a document into the same location as an existing document.

