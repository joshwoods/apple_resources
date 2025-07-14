

- UIKit
- UITextField
-  allowsEditingTextAttributes 

Instance Property

# allowsEditingTextAttributes

A Boolean value that determines whether the user can edit the attributes of the text in the text field.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var allowsEditingTextAttributes: Bool { get set }
```

## Discussion

If this property is set to true, the user may edit the style information of the text. In addition, pasting styled text into the text field retains any embedded style information. If false, the text field prohibits the editing of style information and strips style information from any pasted text. However, you can still set the style information programmatically using the methods of this class.

The default value of this property is false.

## See Also

### Managing the editing behavior

var isEditing: Bool

A Boolean value that indicates whether the text field is currently in edit mode.

var clearsOnBeginEditing: Bool

A Boolean value that determines whether the text field removes old text when editing begins.

var clearsOnInsertion: Bool

A Boolean value that determines whether inserting text replaces the previous contents.

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

