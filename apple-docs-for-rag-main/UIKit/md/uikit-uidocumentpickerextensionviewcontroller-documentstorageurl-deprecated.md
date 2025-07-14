

- UIKit
- UIDocumentPickerExtensionViewController
-  documentStorageURL Deprecated

Instance Property

# documentStorageURL

The root URL for documents provided by the corresponding File Provider extension. (read-only)

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var documentStorageURL: URL? { get }
```

## Discussion

This property returns a subdirectory of the app group container shared by the Document Picker extension and its corresponding File Provider extension. By default, this property holds the value returned by calling the File Provider extension’s documentStorageURL method.

## See Also

### Managing the user interface

func dismissGrantingAccess(to: URL?)

Dismisses the document picker.

Deprecated

var documentPickerMode: UIDocumentPickerMode

The document picker’s file-transfer operation. (read-only)

Deprecated

var originalURL: URL?

The URL of the file to be exported. (read-only)

Deprecated

func prepareForPresentation(in: UIDocumentPickerMode)

Performs any custom configuration of the document picker view controller.

Deprecated

var providerIdentifier: String

An identifier shared by this Document Picker extension and its corresponding File Provider extension. (read-only)

Deprecated

var validTypes: [String]?

An array of valid uniform type identifiers.

Deprecated

