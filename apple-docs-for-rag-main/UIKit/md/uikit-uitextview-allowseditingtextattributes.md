

- UIKit
- UITextView
-  allowsEditingTextAttributes 

Instance Property

# allowsEditingTextAttributes

A Boolean value that indicates whether the text view allows the user to edit style information.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var allowsEditingTextAttributes: Bool { get set }
```

## Discussion

When set to true, the text view allows the user to change the basic styling of the currently selected text. The available style options are listed in the edit menu and only apply to the selection.

The default value of this property is false.

## See Also

### Managing the editing behavior

var isEditable: Bool

A Boolean value that indicates whether the text view is editable.

class let textDidBeginEditingNotification: NSNotification.Name

A notification that alerts observers when an editing session begins in a text view.

class let textDidChangeNotification: NSNotification.Name

A notification that alerts observers when the text in a text view changes.

class let textDidEndEditingNotification: NSNotification.Name

A notification that alerts observers when the editing session ends for a text view.

