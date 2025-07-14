

- AppKit
- NSTextDelegate
-  textDidEndEditing(\_:) 

Instance Method

# textDidEndEditing(\_:)

Informs the delegate that the text object has finished editing (that it has resigned first responder status).

macOS 10.10+

``` source
@MainActor
optional func textDidEndEditing(_ notification: Notification)
```

## Discussion

The name of `aNotification` is didEndEditingNotification.

## See Also

### Editing text

func textShouldBeginEditing(NSText) -> Bool

Invoked when a text object begins to change its text, this method requests permission for `aTextObject` to begin editing.

func textDidBeginEditing(Notification)

Informs the delegate that the text object has begun editing (that the user has begun changing it).

func textShouldEndEditing(NSText) -> Bool

Invoked from a text object’s implementation of resignFirstResponder(), this method requests permission for `aTextObject` to end editing.

