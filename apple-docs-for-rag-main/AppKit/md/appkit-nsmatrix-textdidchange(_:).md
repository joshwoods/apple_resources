

- AppKit
- NSMatrix
-  textDidChange(\_:) 

Instance Method

# textDidChange(\_:)

Invoked when a key-down event or paste operation occurs that changes the receiver’s contents.

macOS

``` source
@MainActor
func textDidChange(_ notification: Notification)
```

## Parameters 

`notification`  

The textDidChangeNotification notification.

## Discussion

This method’s default behavior is to pass this message on to the selected cell (if the selected cell responds to `textDidChange:`) and then to post an textDidChangeNotification along with the receiving object to the default notification center. The posted notification’s user info contains the contents of notification’s user info dictionary, plus an additional key-value pair. The additional key is “`NSFieldEditor`”; the value for this key is the text object that changed.

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

func textShouldEndEditing(NSText) -> Bool

Requests permission to end editing.

func textDidEndEditing(Notification)

Invoked when text editing ends.

