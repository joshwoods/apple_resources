

- AppKit
- NSMatrix
-  textShouldEndEditing(\_:) 

Instance Method

# textShouldEndEditing(\_:)

Requests permission to end editing.

macOS

``` source
@MainActor
func textShouldEndEditing(_ textObject: NSText) -> Bool
```

## Parameters 

`textObject`  

The text object requesting permission to end editing.

## Return Value

true if the text object should proceed to finish editing and resign first responder status. If the delegate returns false, the text object selects all of its text and remains the first responder.

## Discussion

The NSMatrix method returns false if the text field contains invalid contents; otherwise it returns the value passed back from control(_:textShouldEndEditing:).

This method is invoked to let the NSTextField respond to impending loss of first-responder status. This method’s default behavior checks the text field for validity; providing that the field contents are deemed valid, and providing that the delegate responds, control(_:textShouldEndEditing:) is sent to the receiver’s delegate (passing the receiver and `textObject` as parameters).

## See Also

### Related Documentation

var delegate: (any NSMatrixDelegate)?

The delegate for messages from the field editor.

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

func textDidEndEditing(Notification)

Invoked when text editing ends.

