

- UIKit
- UIDocumentMenuViewController
-  init(coder:) Deprecated

Initializer

# init(coder:)

Creates a document menu from data in an unarchiver.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
init?(coder: NSCoder)
```

## See Also

### Creating a document menu

init(documentTypes: [String], in: UIDocumentPickerMode)

Initializes and returns a document menu to import or open the given file types.

Deprecated

init(url: URL, in: UIDocumentPickerMode)

Initializes and returns a document menu to export or move the given document.

Deprecated

