

- UIKit
- UIDocumentBrowserViewController
-  allowedContentTypes Deprecated

Instance Property

# allowedContentTypes

The document types that the browser can open.

iOS 11.0–14.0DeprecatediPadOS 11.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var allowedContentTypes: [String] { get }
```

## Discussion

This property contains an array of uniform type identifiers (UTIs). The document browser can open only documents of the types specified by these UTIs.

The list of UTIs is set when the document browser is first created. This list cannot be changed.If you programmatically create a document browser, this list is set to the value passed to the init(forOpeningFilesWithContentTypes:) method’s `allowedContentTypes` parameter.

If you add a document browser to your project using a storyboard or Interface Builder, this property is calculated based on the the `CFBundleDocumentTypes` key in your app’s `Info.plist` file. For details, see Set the supported document types.

For more about UTIs, see Uniform Type Identifiers Reference.

## See Also

### Deprecated symbols

init(forOpeningFilesWithContentTypes: [String]?)

Initializes and returns a document browser view controller that can open the specified file types.

Deprecated

var recentDocumentsContentTypes: [String]

Content types for browsing recent documents.

Deprecated

func transitionController(forDocumentURL: URL) -> UIDocumentBrowserTransitionController

Creates a transition controller that provides the standard system-loading and segue animations for the document browser.

Deprecated

