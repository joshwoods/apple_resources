

- UIKit
- UIDocumentBrowserViewController
-  revealDocument(at:importIfNeeded:completion:) 

Instance Method

# revealDocument(at:importIfNeeded:completion:)

Reveals, and optionally imports, the document at the provided URL.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func revealDocument(
    at url: URL,
    importIfNeeded: Bool,
    completion: ((URL?, (any Error)?) -> Void)? = nil
)
```

``` source
@MainActor
func revealDocument(
    at url: URL,
    importIfNeeded: Bool
) async throws -> URL
```

## Parameters 

`url`  

The URL of the document to reveal.

`importIfNeeded`  

A Boolean value that determines whether the document browser should import the document.

`completion`  

A completion block with the following parameters:

url  
The new URL of an imported document. Set to `nil` if `shouldImport` is false, or if an error occurs.

error  
If an error occurs, this parameter contains the error information; otherwise, set to `nil`.

## Mentioned in 

Enabling document sharing

## Discussion

Call this method to display a document in the document browser.

If `importIfNeeded` is true, the document browser calls its delegate’s documentBrowser(_:didImportDocumentAt:toDestinationURL:) method (or its documentBrowser(_:failedToImportDocumentAt:error:) method, if an error occurred) before calling the completion handler.

## See Also

### Configuring a document browser

var allowsDocumentCreation: Bool

A Boolean value that determines whether the document browser can create new documents.

var allowsPickingMultipleItems: Bool

A Boolean value that determines whether the user can select and open more than one document at a time.

var contentTypesForRecentDocuments: [UTType]

Content types for browsing recent documents.

