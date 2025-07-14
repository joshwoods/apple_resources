

- UIKit
- UIDocumentPickerDelegate
-  documentPicker(\_:didPickDocumentAt:) Deprecated

Instance Method

# documentPicker(\_:didPickDocumentAt:)

Tells the delegate that the user has selected a document or a destination.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func documentPicker(
    _ controller: UIDocumentPickerViewController,
    didPickDocumentAt url: URL
)
```

Deprecated

Use the documentPicker(_:didPickDocumentsAt:) method instead.

## Parameters 

`controller`  

The document picker that called this method.

`url`  

The URL of the selected document or destination.

## Discussion

The meaning of the provided URL varies depending on the document picker’s mode:

- `UIDocumentPickerModeImport`

The URL refers to a copy of the selected document. This document is a temporary file. It remains available only until your application terminates. To keep a permanent copy, you must move this file to a permanent location inside your sandbox.

- `UIDocumentPickerModeOpen`

The URL refers to the selected document. The provided URL is a security-scoped URL referring to a file outside your app’s sandbox. For more information on working with external, security-scoped URLs, see Requirements.

- `UIDocumentPickerModeExportToService`

The URL refers to the new copy of the exported document at the selected destination. This URL refers to a file outside your app’s sandbox. You cannot access this copy; the URL is passed only to indicate success.

- `UIDocumentPickerModeMoveToService`

The URL refers to the document’s new location. The provided URL is a security-scoped URL referring to a file outside your app’s sandbox. For more information on working with external, security-scoped URLs, see Requirements.

## See Also

### Responding to user actions

func documentPicker(UIDocumentPickerViewController, didPickDocumentsAt: [URL])

Tells the delegate that the user has selected one or more documents.

func documentPickerWasCancelled(UIDocumentPickerViewController)

Tells the delegate that the user canceled the document picker.

