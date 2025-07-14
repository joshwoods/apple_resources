

- UIKit
- UIDocumentPickerViewController
-  init(forOpeningContentTypes:) 

Initializer

# init(forOpeningContentTypes:)

Creates and returns a document picker that can open the types of documents you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
convenience init(forOpeningContentTypes contentTypes: [UTType])
```

## Parameters 

`contentTypes`  

An array of uniform type identifiers for the document picker to display. For more information, see Uniform Type Identifiers.

## See Also

### Creating a document picker

init?(coder: NSCoder)

Returns an initialized object from data in a specified unarchiver.

convenience init(forExporting: [URL])

Creates and returns a document picker that can export the types of documents you specify.

init(forExporting: [URL], asCopy: Bool)

Creates and returns a document picker that can export or copy the types of documents you specify.

init(forOpeningContentTypes: [UTType], asCopy: Bool)

Creates and returns a document picker that can open or copy the types of documents you specify.

