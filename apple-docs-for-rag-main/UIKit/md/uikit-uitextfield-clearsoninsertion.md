

- UIKit
- UITextField
-  clearsOnInsertion 

Instance Property

# clearsOnInsertion

A Boolean value that determines whether inserting text replaces the previous contents.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var clearsOnInsertion: Bool { get set }
```

## Discussion

The default value of this property is false. When the value of this property is true and the text field is in editing mode, the selection UI is hidden and inserting new text clears the contents of the text field and sets the value of this property back to false.

## See Also

### Managing the editing behavior

var isEditing: Bool

A Boolean value that indicates whether the text field is currently in edit mode.

var clearsOnBeginEditing: Bool

A Boolean value that determines whether the text field removes old text when editing begins.

var allowsEditingTextAttributes: Bool

A Boolean value that determines whether the user can edit the attributes of the text in the text field.

enum DidEndEditingReason

Constants that indicate the reason for ending editing in a text field.

class let didEndEditingReasonUserInfoKey: String

A key that indicates the reason for ending editing in a text field.

class let textDidBeginEditingNotification: NSNotification.Name

A notification that alerts observers when an editing session begins in a text field.

class let textDidChangeNotification: NSNotification.Name

A notification that alerts observers when the text in a text field changes.

class let textDidEndEditingNotification: NSNotification.Name

A notification that alerts observers when the editing session ends for a text field.

