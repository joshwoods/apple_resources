

- UIKit
- UIDocumentPickerExtensionViewController
-  validTypes Deprecated

Instance Property

# validTypes

An array of valid uniform type identifiers.

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var validTypes: [String]? { get }
```

## Discussion

While in the `UIDocumentPickerModeImport` or `UIDocumentPickerModeOpen` modes, this property holds an array of valid UTIs; otherwise, it is `nil`.

Check the value of this property before your Document Picker extension displays any files to the user. You should let the user select only files that match at least one of the given UTIs.

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

var providerIdentifier: String

An identifier shared by this Document Picker extension and its corresponding File Provider extension. (read-only)

Deprecated

