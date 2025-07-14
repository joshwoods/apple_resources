

- UIKit
- UIDocumentProperties
-  init(metadata:) 

Initializer

# init(metadata:)

Creates a document properties object from the metadata object you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
init(metadata: LPLinkMetadata)
```

## Parameters 

`metadata`  

Metadata about a document.

## Discussion

If you don’t have a URL backing your document, create a metadata object manually to initialize a document properties object.

## See Also

### Creating a document header

init(url: URL)

Creates a document properties object from document data at the URL you specify.

var metadata: LPLinkMetadata

The document’s metadata.

