

- UIKit
- UIDocumentBrowserViewController
-  transitionController(forDocumentURL:) Deprecated

Instance Method

# transitionController(forDocumentURL:)

Creates a transition controller that provides the standard system-loading and segue animations for the document browser.

iOS 11.0–12.0DeprecatediPadOS 11.0–12.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func transitionController(forDocumentURL documentURL: URL) -> UIDocumentBrowserTransitionController
```

Deprecated

Use transitionController(forDocumentAt:) instead.

## Parameters 

`documentURL`  

The URL of a document. Only use URLs provided by the document browser (for example, URLs passed to the delegate’s documentBrowser(_:didRequestDocumentCreationWithHandler:)method’s completion block).

## Return Value

Returns a newly instantiated transition controller. Its loadingProgress and targetView properties are both set to `nil`.

## Discussion

For the animations to function properly, you must maintain a strong reference to the transition controller until all the animation sequences are complete.

For more about using the transition controller, see UIDocumentBrowserTransitionController.

## See Also

### Deprecated symbols

init(forOpeningFilesWithContentTypes: [String]?)

Initializes and returns a document browser view controller that can open the specified file types.

Deprecated

var recentDocumentsContentTypes: [String]

Content types for browsing recent documents.

Deprecated

var allowedContentTypes: [String]

The document types that the browser can open.

Deprecated

