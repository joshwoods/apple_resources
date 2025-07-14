

- UIKit
- UIDocumentBrowserViewController
-  allowsDocumentCreation 

Instance Property

# allowsDocumentCreation

A Boolean value that determines whether the document browser can create new documents.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var allowsDocumentCreation: Bool { get set }
```

## Mentioned in 

Customizing the browser

## Discussion

The browser creates new documents when the user taps the Add (+) button in the navigation bar. The Add button is enabled only if both the allowsDocumentCreation property is set to true, and the browser delegate implements the documentBrowser(_:didRequestDocumentCreationWithHandler:) method.

By default, this property is set to true.

## See Also

### Configuring a document browser

var allowsPickingMultipleItems: Bool

A Boolean value that determines whether the user can select and open more than one document at a time.

func revealDocument(at: URL, importIfNeeded: Bool, completion: ((URL?, (any Error)?) -> Void)?)

Reveals, and optionally imports, the document at the provided URL.

var contentTypesForRecentDocuments: [UTType]

Content types for browsing recent documents.

