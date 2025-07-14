

- UIKit
- UITextField
-  didEndEditingReasonUserInfoKey 

Type Property

# didEndEditingReasonUserInfoKey

A key that indicates the reason for ending editing in a text field.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
nonisolated
class let didEndEditingReasonUserInfoKey: String
```

## See Also

### Managing the editing behavior

var isEditing: Bool

A Boolean value that indicates whether the text field is currently in edit mode.

var clearsOnBeginEditing: Bool

A Boolean value that determines whether the text field removes old text when editing begins.

var clearsOnInsertion: Bool

A Boolean value that determines whether inserting text replaces the previous contents.

var allowsEditingTextAttributes: Bool

A Boolean value that determines whether the user can edit the attributes of the text in the text field.

enum DidEndEditingReason

Constants that indicate the reason for ending editing in a text field.

class let textDidBeginEditingNotification: NSNotification.Name

A notification that alerts observers when an editing session begins in a text field.

class let textDidChangeNotification: NSNotification.Name

A notification that alerts observers when the text in a text field changes.

class let textDidEndEditingNotification: NSNotification.Name

A notification that alerts observers when the editing session ends for a text field.

