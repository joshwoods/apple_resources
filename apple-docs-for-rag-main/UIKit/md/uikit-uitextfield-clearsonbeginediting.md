

- UIKit
- UITextField
-  clearsOnBeginEditing 

Instance Property

# clearsOnBeginEditing

A Boolean value that determines whether the text field removes old text when editing begins.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var clearsOnBeginEditing: Bool { get set }
```

## Discussion

If this property is set to true, the text field’s previous text is cleared when the user selects the text field to begin editing. If false, the text field places an insertion point at the place where the user tapped the field.

Note

Even if this property is set to true, the text field delegate can override this behavior by returning false from its textFieldShouldClear(_:) method.

## See Also

### Managing the editing behavior

var isEditing: Bool

A Boolean value that indicates whether the text field is currently in edit mode.

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

