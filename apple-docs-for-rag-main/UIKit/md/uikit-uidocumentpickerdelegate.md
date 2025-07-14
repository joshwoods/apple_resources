

- UIKit
-  UIDocumentPickerDelegate 

Protocol

# UIDocumentPickerDelegate

A set of methods for tracking when the user selects a document or destination, or cancels the operation.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
protocol UIDocumentPickerDelegate : NSObjectProtocol
```

## Topics

### Responding to user actions

func documentPicker(UIDocumentPickerViewController, didPickDocumentsAt: [URL])

Tells the delegate that the user has selected one or more documents.

func documentPickerWasCancelled(UIDocumentPickerViewController)

Tells the delegate that the user canceled the document picker.

func documentPicker(UIDocumentPickerViewController, didPickDocumentAt: URL)

Tells the delegate that the user has selected a document or a destination.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Getting the user-selected document

var delegate: (any UIDocumentPickerDelegate)?

An object that acts as the delegate of the view controller.

var allowsMultipleSelection: Bool

A Boolean value that determines whether the user can select more than one document at a time.

var directoryURL: URL?

The initial directory that the document picker displays.

