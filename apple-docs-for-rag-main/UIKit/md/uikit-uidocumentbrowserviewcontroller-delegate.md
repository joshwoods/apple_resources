

- UIKit
- UIDocumentBrowserViewController
-  delegate 

Instance Property

# delegate

The document browser’s delegate.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIDocumentBrowserViewControllerDelegate)? { get set }
```

## Discussion

The delegate object must implement the UIDocumentBrowserViewControllerDelegate protocol.

## See Also

### Responding to browser events

protocol UIDocumentBrowserViewControllerDelegate

The protocol you implement to respond as the user interacts with the document browser.

func importDocument(at: URL, nextToDocumentAt: URL, mode: UIDocumentBrowserViewController.ImportMode, completionHandler: (URL?, (any Error)?) -> Void)

Imports a document into the same location as an existing document.

