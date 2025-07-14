

- AppKit
- NSTextDelegate
-  textShouldBeginEditing(\_:) 

Instance Method

# textShouldBeginEditing(\_:)

Invoked when a text object begins to change its text, this method requests permission for `aTextObject` to begin editing.

macOS

``` source
@MainActor
optional func textShouldBeginEditing(_ textObject: NSText) -> Bool
```

## Discussion

If the delegate returns true, the text object proceeds to make changes. If the delegate returns false, the text object abandons the editing operation. This method is also invoked when the user drags and drops a file onto the text object.

## See Also

### Related Documentation

func becomeFirstResponder() -> Bool

Notifies the receiver that it’s about to become first responder in its NSWindow.

func makeFirstResponder(NSResponder?) -> Bool

Attempts to make a given responder the first responder for the window.

### Editing text

func textDidBeginEditing(Notification)

Informs the delegate that the text object has begun editing (that the user has begun changing it).

func textShouldEndEditing(NSText) -> Bool

Invoked from a text object’s implementation of resignFirstResponder(), this method requests permission for `aTextObject` to end editing.

func textDidEndEditing(Notification)

Informs the delegate that the text object has finished editing (that it has resigned first responder status).

