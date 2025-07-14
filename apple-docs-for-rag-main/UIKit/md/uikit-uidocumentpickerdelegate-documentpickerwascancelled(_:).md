

- UIKit
- UIDocumentPickerDelegate
-  documentPickerWasCancelled(\_:) 

Instance Method

# documentPickerWasCancelled(\_:)

Tells the delegate that the user canceled the document picker.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func documentPickerWasCancelled(_ controller: UIDocumentPickerViewController)
```

## Parameters 

`controller`  

The document picker that called this method.

## Mentioned in 

Providing access to directories

## See Also

### Responding to user actions

func documentPicker(UIDocumentPickerViewController, didPickDocumentsAt: [URL])

Tells the delegate that the user has selected one or more documents.

func documentPicker(UIDocumentPickerViewController, didPickDocumentAt: URL)

Tells the delegate that the user has selected a document or a destination.

Deprecated

