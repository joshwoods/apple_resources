

- UIKit
- UIDocumentBrowserViewController
-  init(forOpeningFilesWithContentTypes:) Deprecated

Initializer

# init(forOpeningFilesWithContentTypes:)

Initializes and returns a document browser view controller that can open the specified file types.

iOS 11.0–14.0DeprecatediPadOS 11.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
init(forOpeningFilesWithContentTypes allowedContentTypes: [String]?)
```

Deprecated

Use init(forOpening:) instead.

## Parameters 

`allowedContentTypes`  

An array of uniform type identifiers (UTIs). The document browser can open only the document types that these UTIs specify. If you pass `nil`, the browser uses the document types that the `CFBundleDocumentTypes` key specifies in the app’s `Info.plist` file.

For detailed instructions about setting the `CFBundleDocumentTypes` key, see the Set the supported document types section of Setting up a document browser app.

For more information about UTIs, see Uniform Type Identifiers.

## Return Value

Returns a newly initialized document browser view controller.

## Mentioned in 

Customizing the browser

## See Also

### Deprecated symbols

var recentDocumentsContentTypes: [String]

Content types for browsing recent documents.

Deprecated

var allowedContentTypes: [String]

The document types that the browser can open.

Deprecated

func transitionController(forDocumentURL: URL) -> UIDocumentBrowserTransitionController

Creates a transition controller that provides the standard system-loading and segue animations for the document browser.

Deprecated

