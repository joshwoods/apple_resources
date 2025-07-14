

- UIKit
- UIDocumentBrowserViewController
-  UIDocumentBrowserViewController.ImportMode 

Enumeration

# UIDocumentBrowserViewController.ImportMode

The document browser’s import modes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum ImportMode
```

## Mentioned in 

Customizing a document-based app’s launch experience

## Topics

### Constants

case copy

A mode indicating that the file should be copied into its new location (the original file is left unchanged).

case move

A mode indicating that the file should be moved to its new location (the original file should be deleted).

case none

A mode indicating that the document can’t be imported.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating new documents

func documentBrowser(UIDocumentBrowserViewController, didRequestDocumentCreationWithHandler: (URL?, UIDocumentBrowserViewController.ImportMode) -> Void)

Asks the delegate to create a new document.

func documentBrowser(UIDocumentBrowserViewController, didImportDocumentAt: URL, toDestinationURL: URL)

Tells the delegate that a document has been successfully imported.

func documentBrowser(UIDocumentBrowserViewController, failedToImportDocumentAt: URL, error: (any Error)?)

Tells the delegate that the document browser failed to import the specified document.

