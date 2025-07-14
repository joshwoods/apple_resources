

- UIKit
- UIDocumentPickerViewController
-  delegate 

Instance Property

# delegate

An object that acts as the delegate of the view controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIDocumentPickerDelegate)? { get set }
```

## Discussion

The delegate must adopt the UIDocumentPickerDelegate protocol.

## See Also

### Getting the user-selected document

protocol UIDocumentPickerDelegate

A set of methods for tracking when the user selects a document or destination, or cancels the operation.

var allowsMultipleSelection: Bool

A Boolean value that determines whether the user can select more than one document at a time.

var directoryURL: URL?

The initial directory that the document picker displays.

