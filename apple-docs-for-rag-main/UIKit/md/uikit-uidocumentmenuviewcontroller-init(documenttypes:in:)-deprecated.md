

- UIKit
- UIDocumentMenuViewController
-  init(documentTypes:in:) Deprecated

Initializer

# init(documentTypes:in:)

Initializes and returns a document menu to import or open the given file types.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
init(
    documentTypes allowedUTIs: [String],
    in mode: UIDocumentPickerMode
)
```

## Parameters 

`allowedUTIs`  

An array of uniform type identifiers. UTIs are strings that uniquely identify a file’s type. For more information, see Uniform Type Identifiers Overview.

`mode`  

The type of file transfer operation the document picker performs. This argument accepts only the UIDocumentPickerMode.import or UIDocumentPickerMode.open mode.

## Return Value

Returns an initialized `UIDocumentMenuViewController` object, or `nil` if the object could not be successfully initialized.

## Discussion

The UTI array defines the type of documents that can be imported or opened. The resulting document menu displays all the document pickers appropriate for the given document types and mode.

## See Also

### Creating a document menu

init(url: URL, in: UIDocumentPickerMode)

Initializes and returns a document menu to export or move the given document.

Deprecated

init?(coder: NSCoder)

Creates a document menu from data in an unarchiver.

Deprecated

