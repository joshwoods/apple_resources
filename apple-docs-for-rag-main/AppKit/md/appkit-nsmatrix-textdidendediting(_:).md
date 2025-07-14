

- AppKit
- NSMatrix
-  textDidEndEditing(\_:) 

Instance Method

# textDidEndEditing(\_:)

Invoked when text editing ends.

macOS

``` source
@MainActor
func textDidEndEditing(_ notification: Notification)
```

## Parameters 

`notification`  

The textDidEndEditingNotification notification.

## Discussion

This method’s default behavior is to post an textDidEndEditingNotification along with the receiving object to the default notification center. The posted notification’s user info contains the contents of notification’s user info dictionary, plus an additional key-value pair. The additional key is “`NSFieldEditor`”; the value for this key is the text object that began editing. After posting the notification, NSMatrix sends an endEditing(_:) message to the selected cell, draws and makes the selected cell key, and then takes the appropriate action based on which key was used to end editing (Return, Tab, or Back-Tab).

## See Also

### Editing Text in Cells

func selectText(Any?)

Selects text in the currently selected cell or in the key cell.

func selectText(atRow: Int, column: Int) -> NSCell?

Selects the text in the cell at the specified location and returns the cell.

func textShouldBeginEditing(NSText) -> Bool

Requests permission to begin editing text.

func textDidBeginEditing(Notification)

Invoked when there’s a change in the text after the receiver gains first responder status.

func textDidChange(Notification)

Invoked when a key-down event or paste operation occurs that changes the receiver’s contents.

func textShouldEndEditing(NSText) -> Bool

Requests permission to end editing.

