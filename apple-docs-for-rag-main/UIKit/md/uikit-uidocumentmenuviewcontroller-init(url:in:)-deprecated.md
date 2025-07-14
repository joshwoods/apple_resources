

- UIKit
- UIDocumentMenuViewController
-  init(url:in:) Deprecated

Initializer

# init(url:in:)

Initializes and returns a document menu to export or move the given document.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
init(
    url: URL,
    in mode: UIDocumentPickerMode
)
```

## Parameters 

`url`  

The document to be exported or moved.

`mode`  

The type of file-transfer operation that the document picker performs. This argument accepts only the UIDocumentPickerModeExportToService or UIDocumentPickerModeMoveToService mode.

## Return Value

Returns an initialized `UIDocumentMenuViewController` object, or `nil` if the object could not be successfully initialized.

## Discussion

The resulting document menu displays all the document pickers appropriate for the given mode.

## See Also

### Creating a document menu

init(documentTypes: [String], in: UIDocumentPickerMode)

Initializes and returns a document menu to import or open the given file types.

Deprecated

init?(coder: NSCoder)

Creates a document menu from data in an unarchiver.

Deprecated

