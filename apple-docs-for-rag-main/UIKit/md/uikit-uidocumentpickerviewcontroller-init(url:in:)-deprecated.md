

- UIKit
- UIDocumentPickerViewController
-  init(url:in:) Deprecated

Initializer

# init(url:in:)

Initializes and returns a document picker that can export or copy the specified document.

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
init(
    url: URL,
    in mode: UIDocumentPickerMode
)
```

Deprecated

Use init(forExporting:) or init(forExporting:asCopy:) instead.

## Parameters 

`url`  

The document that the document picker exports or moves.

`mode`  

The type of file-transfer operation that the document picker performs. This argument accepts only the UIDocumentPickerMode.exportToService or UIDocumentPickerMode.moveToService mode.

## Return Value

Returns an initialized `UIDocumentPickerViewController` object, or `nil` if the object could not be successfully initialized.

## Discussion

In iOS 10 and earlier, this method returns the document picker view controller from the most recently used Document Provider extension. If no valid Document Provider can be found, it defaults back to iCloud Drive.

In iOS 11 and later, it returns the standard browser interface. This interface is the same one used by the UIDocumentBrowserViewController class.

## See Also

### Deprecated

init(documentTypes: [String], in: UIDocumentPickerMode)

Creates and returns a document picker that can open or copy the specified file types.

Deprecated

init(urls: [URL], in: UIDocumentPickerMode)

Creates and returns a document picker that can export or move the specified documents.

Deprecated

