

- UIKit
- UIDocumentPickerViewController
-  init(documentTypes:in:) Deprecated

Initializer

# init(documentTypes:in:)

Creates and returns a document picker that can open or copy the specified file types.

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
init(
    documentTypes allowedUTIs: [String],
    in mode: UIDocumentPickerMode
)
```

Deprecated

Use init(forOpeningContentTypes:) or init(forOpeningContentTypes:asCopy:) instead.

## Parameters 

`allowedUTIs`  

An array of uniform type identifiers (UTIs). UTIs are strings that uniquely identify a file’s type. For more information, see Uniform Type Identifiers Overview.

`mode`  

The type of file-transfer operation that the document picker performs. This argument accepts only the UIDocumentPickerMode.import or UIDocumentPickerMode.open mode.

## Return Value

Returns an initialized `UIDocumentPickerViewController` object, or `nil` if the object could not be successfully initialized.

## Discussion

In iOS 10 and earlier, this method returns the document picker view controller from the most recently used Document Provider extension. If no valid Document Provider can be found, it defaults back to iCloud Drive.

In iOS 11 and later, it returns the standard browser interface. This interface is the same one used by the UIDocumentBrowserViewController class.

## See Also

### Deprecated

init(url: URL, in: UIDocumentPickerMode)

Initializes and returns a document picker that can export or copy the specified document.

Deprecated

init(urls: [URL], in: UIDocumentPickerMode)

Creates and returns a document picker that can export or move the specified documents.

Deprecated

