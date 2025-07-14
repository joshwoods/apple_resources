

- UIKit
- UIDocumentPickerExtensionViewController
-  prepareForPresentation(in:) Deprecated

Instance Method

# prepareForPresentation(in:)

Performs any custom configuration of the document picker view controller.

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func prepareForPresentation(in mode: UIDocumentPickerMode)
```

## Parameters 

`mode`  

The type of file-transfer operation that the document picker performs. For a list of valid modes, see `Document Picker Modes`.

## Discussion

The system calls this method when a host app presents a document picker view controller for your Document Picker extension. Override this method to provide a custom user interface based on the provided mode.

Different modes may require different user interfaces. For example, the UIDocumentPickerModeImport and UIDocumentPickerModeOpen modes should let the user explore the available documents, whereas the UIDocumentPickerModeExportToService and UIDocumentPickerModeMoveToService modes let the user select the destination.

When overriding this method, examine the mode and present an appropriate user interface for the task at hand. If the differences between the modes are significant, consider creating separate child view controllers for each mode and then present the appropriate child in this method.

If your extension can manage multiple file types, check the validTypes property and make sure you are presenting only files that match one or more of the specified types.

## See Also

### Managing the user interface

func dismissGrantingAccess(to: URL?)

Dismisses the document picker.

Deprecated

var documentPickerMode: UIDocumentPickerMode

The document picker’s file-transfer operation. (read-only)

Deprecated

var documentStorageURL: URL?

The root URL for documents provided by the corresponding File Provider extension. (read-only)

Deprecated

var originalURL: URL?

The URL of the file to be exported. (read-only)

Deprecated

var providerIdentifier: String

An identifier shared by this Document Picker extension and its corresponding File Provider extension. (read-only)

Deprecated

var validTypes: [String]?

An array of valid uniform type identifiers.

Deprecated

