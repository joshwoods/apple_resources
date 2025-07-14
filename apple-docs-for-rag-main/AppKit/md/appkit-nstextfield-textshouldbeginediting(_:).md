

- AppKit
- NSTextField
-  textShouldBeginEditing(\_:) 

Instance Method

# textShouldBeginEditing(\_:)

Requests permission to begin editing a text object.

macOS

``` source
@MainActor
func textShouldBeginEditing(_ textObject: NSText) -> Bool
```

## Parameters 

`textObject`  

The object to begin editing.

## Return Value

true if editing can begin; otherwise, false.

## Discussion

If the text field isn’t editable, this method returns false immediately. If the text field is editable and its delegate responds to control(_:textShouldBeginEditing:), this method invokes that method and returns the result. Otherwise, it returns true to allow editing to occur. See NSControl for more information about the text delegate method.

## See Also

### Implementing Delegate Methods

func textDidBeginEditing(Notification)

Posts a notification to the default notification center that the text is about to go into edit mode.

func textDidChange(Notification)

Posts a notification when the text changes, and forwards the message to the text field’s cell if it responds.

func textShouldEndEditing(NSText) -> Bool

Performs validation on the text field’s new value.

func textDidEndEditing(Notification)

Posts a notification when the text is no longer in edit mode.

