

- UIKit
- UITextView
-  textDidChangeNotification 

Type Property

# textDidChangeNotification

A notification that alerts observers when the text in a text view changes.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
nonisolated
class let textDidChangeNotification: NSNotification.Name
```

## Discussion

The affected view is stored in the `object` parameter of the notification. The `userInfo` dictionary is not used.

## See Also

### Managing the editing behavior

var isEditable: Bool

A Boolean value that indicates whether the text view is editable.

var allowsEditingTextAttributes: Bool

A Boolean value that indicates whether the text view allows the user to edit style information.

class let textDidBeginEditingNotification: NSNotification.Name

A notification that alerts observers when an editing session begins in a text view.

class let textDidEndEditingNotification: NSNotification.Name

A notification that alerts observers when the editing session ends for a text view.

