

- UIKit
- UITextView
-  isEditable 

Instance Property

# isEditable

A Boolean value that indicates whether the text view is editable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var isEditable: Bool { get set }
```

## Discussion

The default value of this property is true.

## See Also

### Managing the editing behavior

var allowsEditingTextAttributes: Bool

A Boolean value that indicates whether the text view allows the user to edit style information.

class let textDidBeginEditingNotification: NSNotification.Name

A notification that alerts observers when an editing session begins in a text view.

class let textDidChangeNotification: NSNotification.Name

A notification that alerts observers when the text in a text view changes.

class let textDidEndEditingNotification: NSNotification.Name

A notification that alerts observers when the editing session ends for a text view.

