

- AppKit
- NSTextField
-  textShouldEndEditing(\_:) 

Instance Method

# textShouldEndEditing(\_:)

Performs validation on the text field’s new value.

macOS

``` source
@MainActor
func textShouldEndEditing(_ textObject: NSText) -> Bool
```

## Parameters 

`textObject`  

The text object that requests permission to end editing.

## Return Value

true if the new value is valid; otherwise, false.

## Discussion

This method validates the text field’s new value using the `NSCell` method isEntryAcceptable:. If the new value is valid and the delegate responds to control(_:textShouldEndEditing:), this method invokes that method and returns the result. If the delegate returns false, the system beeps to indicate that the text field can’t validate the text. See NSControl for more information about the text delegate method.

## See Also

### Implementing Delegate Methods

func textShouldBeginEditing(NSText) -> Bool

Requests permission to begin editing a text object.

func textDidBeginEditing(Notification)

Posts a notification to the default notification center that the text is about to go into edit mode.

func textDidChange(Notification)

Posts a notification when the text changes, and forwards the message to the text field’s cell if it responds.

func textDidEndEditing(Notification)

Posts a notification when the text is no longer in edit mode.

