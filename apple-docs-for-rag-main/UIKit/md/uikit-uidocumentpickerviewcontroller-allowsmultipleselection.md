

- UIKit
- UIDocumentPickerViewController
-  allowsMultipleSelection 

Instance Property

# allowsMultipleSelection

A Boolean value that determines whether the user can select more than one document at a time.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var allowsMultipleSelection: Bool { get set }
```

## Discussion

By default, this property is false.

## See Also

### Getting the user-selected document

var delegate: (any UIDocumentPickerDelegate)?

An object that acts as the delegate of the view controller.

protocol UIDocumentPickerDelegate

A set of methods for tracking when the user selects a document or destination, or cancels the operation.

var directoryURL: URL?

The initial directory that the document picker displays.

