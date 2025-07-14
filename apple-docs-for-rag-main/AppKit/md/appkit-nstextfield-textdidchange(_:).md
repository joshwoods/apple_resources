

- AppKit
- NSTextField
-  textDidChange(\_:) 

Instance Method

# textDidChange(\_:)

Posts a notification when the text changes, and forwards the message to the text field’s cell if it responds.

macOS

``` source
@MainActor
func textDidChange(_ notification: Notification)
```

## Parameters 

`notification`  

The textDidChangeNotification notification to post to the default notification center.

## Discussion

This method causes the text field’s delegate to receive a controlTextDidChange: message. See the NSControl class specification for more information about the text delegate method.

## See Also

### Implementing Delegate Methods

func textShouldBeginEditing(NSText) -> Bool

Requests permission to begin editing a text object.

func textDidBeginEditing(Notification)

Posts a notification to the default notification center that the text is about to go into edit mode.

func textShouldEndEditing(NSText) -> Bool

Performs validation on the text field’s new value.

func textDidEndEditing(Notification)

Posts a notification when the text is no longer in edit mode.

