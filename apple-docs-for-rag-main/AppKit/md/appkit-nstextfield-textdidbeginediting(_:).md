

- AppKit
- NSTextField
-  textDidBeginEditing(\_:) 

Instance Method

# textDidBeginEditing(\_:)

Posts a notification to the default notification center that the text is about to go into edit mode.

macOS

``` source
@MainActor
func textDidBeginEditing(_ notification: Notification)
```

## Parameters 

`notification`  

The textDidBeginEditingNotification notification to post to the default notification center.

## Discussion

This action causes the text field’s delegate to receive a controlTextDidBeginEditing: message. See NSControl for more information about the text delegate method.

## See Also

### Implementing Delegate Methods

func textShouldBeginEditing(NSText) -> Bool

Requests permission to begin editing a text object.

func textDidChange(Notification)

Posts a notification when the text changes, and forwards the message to the text field’s cell if it responds.

func textShouldEndEditing(NSText) -> Bool

Performs validation on the text field’s new value.

func textDidEndEditing(Notification)

Posts a notification when the text is no longer in edit mode.

