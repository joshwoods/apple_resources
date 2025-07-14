

- UIKit
- UIDocumentPickerViewController
-  init(forExporting:) 

Initializer

# init(forExporting:)

Creates and returns a document picker that can export the types of documents you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
convenience init(forExporting urls: [URL])
```

## Parameters 

`urls`  

An array of documents that the document picker exports.

## See Also

### Creating a document picker

init?(coder: NSCoder)

Returns an initialized object from data in a specified unarchiver.

init(forExporting: [URL], asCopy: Bool)

Creates and returns a document picker that can export or copy the types of documents you specify.

convenience init(forOpeningContentTypes: [UTType])

Creates and returns a document picker that can open the types of documents you specify.

init(forOpeningContentTypes: [UTType], asCopy: Bool)

Creates and returns a document picker that can open or copy the types of documents you specify.

