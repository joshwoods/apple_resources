

- UIKit
- UIDocumentBrowserViewController
-  recentDocumentsContentTypes Deprecated

Instance Property

# recentDocumentsContentTypes

Content types for browsing recent documents.

iOS 11.0–14.0DeprecatediPadOS 11.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var recentDocumentsContentTypes: [String] { get }
```

Deprecated

Use contentTypesForRecentDocuments instead.

## Discussion

The default list is the same as the list of content types provided to the initializer, or the types defined in CFBundleDocumentTypes in the app’s `Info.plist` file.

You can define a subset of these types using the key `UIDocumentBrowserRecentDocumentContentTypes` in the app’s `Info.plist` file.

## See Also

### Deprecated symbols

init(forOpeningFilesWithContentTypes: [String]?)

Initializes and returns a document browser view controller that can open the specified file types.

Deprecated

var allowedContentTypes: [String]

The document types that the browser can open.

Deprecated

func transitionController(forDocumentURL: URL) -> UIDocumentBrowserTransitionController

Creates a transition controller that provides the standard system-loading and segue animations for the document browser.

Deprecated

