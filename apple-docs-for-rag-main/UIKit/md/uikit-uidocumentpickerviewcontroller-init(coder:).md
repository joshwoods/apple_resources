

- UIKit
- UIDocumentPickerViewController
-  init(coder:) 

Initializer

# init(coder:)

Returns an initialized object from data in a specified unarchiver.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init?(coder: NSCoder)
```

## Parameters 

`coder`  

An unarchiver object.

## See Also

### Creating a document picker

convenience init(forExporting: [URL])

Creates and returns a document picker that can export the types of documents you specify.

init(forExporting: [URL], asCopy: Bool)

Creates and returns a document picker that can export or copy the types of documents you specify.

convenience init(forOpeningContentTypes: [UTType])

Creates and returns a document picker that can open the types of documents you specify.

init(forOpeningContentTypes: [UTType], asCopy: Bool)

Creates and returns a document picker that can open or copy the types of documents you specify.

