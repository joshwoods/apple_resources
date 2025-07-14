

- AppKit
- NSMatrix
-  textShouldBeginEditing(\_:) 

Instance Method

# textShouldBeginEditing(\_:)

Requests permission to begin editing text.

macOS

``` source
@MainActor
func textShouldBeginEditing(_ textObject: NSText) -> Bool
```

## Parameters 

`textObject`  

The text object requesting permission to begin editing.

## Return Value

true if the text object should proceed to make changes. If the delegate returns false, the text object abandons the editing operation.

## Discussion

The default behavior of this method is to return the value obtained from control(_:textShouldBeginEditing:), unless the delegate doesn’t respond to that method, in which case it returns true, thereby allowing text editing to proceed.

This method is invoked to let the NSTextField respond to impending changes to its text. This method’s default behavior is to send control(_:textShouldBeginEditing:) to the receiver’s delegate (passing the receiver and `textObject` as parameters).

## See Also

### Related Documentation

var delegate: (any NSMatrixDelegate)?

The delegate for messages from the field editor.

### Editing Text in Cells

func selectText(Any?)

Selects text in the currently selected cell or in the key cell.

func selectText(atRow: Int, column: Int) -> NSCell?

Selects the text in the cell at the specified location and returns the cell.

func textDidBeginEditing(Notification)

Invoked when there’s a change in the text after the receiver gains first responder status.

func textDidChange(Notification)

Invoked when a key-down event or paste operation occurs that changes the receiver’s contents.

func textShouldEndEditing(NSText) -> Bool

Requests permission to end editing.

func textDidEndEditing(Notification)

Invoked when text editing ends.

