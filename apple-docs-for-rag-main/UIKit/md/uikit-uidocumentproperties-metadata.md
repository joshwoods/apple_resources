

- UIKit
- UIDocumentProperties
-  metadata 

Instance Property

# metadata

The document’s metadata.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var metadata: LPLinkMetadata { get set }
```

## Discussion

If you initialize the document properties object using init(url:), UIKit generates this metadata automatically. Typically, you don’t need to access the value of this property directly because UIKit updates the metadata asynchronously to display the latest information in the document header.

If you initialize the document properties object using init(metadata:), you can use this property to manually set metadata if it requires an update.

## See Also

### Creating a document header

init(url: URL)

Creates a document properties object from document data at the URL you specify.

init(metadata: LPLinkMetadata)

Creates a document properties object from the metadata object you specify.

