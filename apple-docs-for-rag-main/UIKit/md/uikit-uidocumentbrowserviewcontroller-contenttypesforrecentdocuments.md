

- UIKit
- UIDocumentBrowserViewController
-  contentTypesForRecentDocuments 

Instance Property

# contentTypesForRecentDocuments

Content types for browsing recent documents.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
var contentTypesForRecentDocuments: [UTType] { get }
```

## Discussion

The default list is the same as the list of content types you provide to the initializer, or the types you define in CFBundleDocumentTypes in the app’s `Info.plist` file.

You can define a subset of these types using the `UIDocumentBrowserRecentDocumentContentTypes` key in the app’s `Info.plist` file.

## See Also

### Configuring a document browser

var allowsDocumentCreation: Bool

A Boolean value that determines whether the document browser can create new documents.

var allowsPickingMultipleItems: Bool

A Boolean value that determines whether the user can select and open more than one document at a time.

func revealDocument(at: URL, importIfNeeded: Bool, completion: ((URL?, (any Error)?) -> Void)?)

Reveals, and optionally imports, the document at the provided URL.

