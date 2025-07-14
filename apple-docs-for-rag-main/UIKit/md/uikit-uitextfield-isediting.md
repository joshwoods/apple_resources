

- UIKit
- UITextField
-  isEditing 

Instance Property

# isEditing

A Boolean value that indicates whether the text field is currently in edit mode.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isEditing: Bool { get }
```

## Discussion

This property is set to true when the user begins editing text in this text field, and it is set to false again when editing ends. The text field notifies its delegate when editing begins and ends.

## See Also

### Managing the editing behavior

var clearsOnBeginEditing: Bool

A Boolean value that determines whether the text field removes old text when editing begins.

var clearsOnInsertion: Bool

A Boolean value that determines whether inserting text replaces the previous contents.

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

