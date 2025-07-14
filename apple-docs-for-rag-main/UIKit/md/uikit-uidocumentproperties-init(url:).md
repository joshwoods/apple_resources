

- UIKit
- UIDocumentProperties
-  init(url:) 

Initializer

# init(url:)

Creates a document properties object from document data at the URL you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
init(url: URL)
```

## Parameters 

`url`  

The URL that points to the document data.

## Discussion

When you initialize a document properties object with a URL, UIKit automatically finds the corresponding metadata and stores it in the document properties object’s metadata property.

## See Also

### Creating a document header

init(metadata: LPLinkMetadata)

Creates a document properties object from the metadata object you specify.

var metadata: LPLinkMetadata

The document’s metadata.

