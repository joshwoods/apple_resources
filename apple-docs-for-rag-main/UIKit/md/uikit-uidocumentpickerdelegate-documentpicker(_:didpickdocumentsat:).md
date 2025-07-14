

- UIKit
- UIDocumentPickerDelegate
-  documentPicker(\_:didPickDocumentsAt:) 

Instance Method

# documentPicker(\_:didPickDocumentsAt:)

Tells the delegate that the user has selected one or more documents.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func documentPicker(
    _ controller: UIDocumentPickerViewController,
    didPickDocumentsAt urls: [URL]
)
```

## Parameters 

`controller`  

The document picker that called this method.

`urls`  

The URLs of the selected documents.

## Mentioned in 

Providing access to directories

## Discussion

The meaning of the provided URLs varies depending on the document picker’s mode:

- `UIDocumentPickerModeImport`

The URLs refer to a copy of the selected documents. These documents are temporary files. They remain available only until your application terminates. To keep a permanent copy, move these files to a permanent location inside your sandbox.

- `UIDocumentPickerModeOpen`

The URLs refer to the selected documents.

- `UIDocumentPickerModeExportToService`

The URLs refer to new copies of the exported documents at the selected destination.

- `UIDocumentPickerModeMoveToService`

The URLs refer to the documents’ new locations.

The provided URLs are security-scoped, referring to files outside your app’s sandbox. For more about working with external, security-scoped URLs, see Requirements in the Document Picker Programming Guide.

## See Also

### Responding to user actions

func documentPickerWasCancelled(UIDocumentPickerViewController)

Tells the delegate that the user canceled the document picker.

func documentPicker(UIDocumentPickerViewController, didPickDocumentAt: URL)

Tells the delegate that the user has selected a document or a destination.

Deprecated

