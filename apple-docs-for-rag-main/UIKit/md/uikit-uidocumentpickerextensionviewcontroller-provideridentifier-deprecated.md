

- UIKit
- UIDocumentPickerExtensionViewController
-  providerIdentifier Deprecated

Instance Property

# providerIdentifier

An identifier shared by this Document Picker extension and its corresponding File Provider extension. (read-only)

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var providerIdentifier: String { get }
```

## Discussion

Both the Document Picker View Controller extension and the File Provider extension should pass this identifier to their file coordinator’s `setPurposeIdentifier:` method. This approach helps coordinate the read and write operations between the two extensions, preventing possible deadlocks.

This property holds the value returned by calling the File Provider extension’s providerIdentifier method.

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

func prepareForPresentation(in: UIDocumentPickerMode)

Performs any custom configuration of the document picker view controller.

Deprecated

var validTypes: [String]?

An array of valid uniform type identifiers.

Deprecated

