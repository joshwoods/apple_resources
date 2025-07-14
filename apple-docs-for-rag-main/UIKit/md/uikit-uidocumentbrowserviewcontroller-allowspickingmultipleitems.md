

- UIKit
- UIDocumentBrowserViewController
-  allowsPickingMultipleItems 

Instance Property

# allowsPickingMultipleItems

A Boolean value that determines whether the user can select and open more than one document at a time.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var allowsPickingMultipleItems: Bool { get set }
```

## Mentioned in 

Customizing the browser

## Discussion

By default, this property is set to false.

## See Also

### Configuring a document browser

var allowsDocumentCreation: Bool

A Boolean value that determines whether the document browser can create new documents.

func revealDocument(at: URL, importIfNeeded: Bool, completion: ((URL?, (any Error)?) -> Void)?)

Reveals, and optionally imports, the document at the provided URL.

var contentTypesForRecentDocuments: [UTType]

Content types for browsing recent documents.

