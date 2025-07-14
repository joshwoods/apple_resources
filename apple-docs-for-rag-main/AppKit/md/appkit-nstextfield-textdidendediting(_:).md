

- AppKit
- NSTextField
-  textDidEndEditing(\_:) 

Instance Method

# textDidEndEditing(\_:)

Posts a notification when the text is no longer in edit mode.

macOS

``` source
@MainActor
func textDidEndEditing(_ notification: Notification)
```

## Parameters 

`notification`  

The textDidEndEditingNotification to post to the default notification center.

## Discussion

After validating the new value, this method posts a textDidEndEditingNotification to the default notification center, which causes the text field’s delegate to receive a controlTextDidEndEditing: message. This method then sends endEditing(_:) to the text field’s cell and handles the key that causes editing to end as follows:

- If the user ends editing by pressing Return, this method tries to send the text field’s action to its target. If unsuccessful, it sends performKeyEquivalent(with:) to its `NSView`, for example, to handle the default button on a panel. If that also fails, the text field selects its text.

- If the user ends editing by pressing Tab or Shift-Tab, the text field tries to have its `NSWindow` object select its next or previous key view, using the `NSWindow` method selectKeyView(following:) or selectKeyView(preceding:). If unsuccessful, the text field selects its text.

See NSControl for more information about the text delegate method.

## See Also

### Implementing Delegate Methods

func textShouldBeginEditing(NSText) -> Bool

Requests permission to begin editing a text object.

func textDidBeginEditing(Notification)

Posts a notification to the default notification center that the text is about to go into edit mode.

func textDidChange(Notification)

Posts a notification when the text changes, and forwards the message to the text field’s cell if it responds.

func textShouldEndEditing(NSText) -> Bool

Performs validation on the text field’s new value.

