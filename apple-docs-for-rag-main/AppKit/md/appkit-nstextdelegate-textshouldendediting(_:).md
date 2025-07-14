

- AppKit
- NSTextDelegate
-  textShouldEndEditing(\_:) 

Instance Method

# textShouldEndEditing(\_:)

Invoked from a text object’s implementation of resignFirstResponder(), this method requests permission for `aTextObject` to end editing.

macOS

``` source
@MainActor
optional func textShouldEndEditing(_ textObject: NSText) -> Bool
```

## Discussion

If the delegate returns true, the text object proceeds to finish editing and resign first responder status. If the delegate returns false, the text object selects all of its text and remains the first responder.

## See Also

### Related Documentation

func resignFirstResponder() -> Bool

Notifies the receiver that it’s been asked to relinquish its status as first responder in its window.

### Editing text

func textShouldBeginEditing(NSText) -> Bool

Invoked when a text object begins to change its text, this method requests permission for `aTextObject` to begin editing.

func textDidBeginEditing(Notification)

Informs the delegate that the text object has begun editing (that the user has begun changing it).

func textDidEndEditing(Notification)

Informs the delegate that the text object has finished editing (that it has resigned first responder status).

