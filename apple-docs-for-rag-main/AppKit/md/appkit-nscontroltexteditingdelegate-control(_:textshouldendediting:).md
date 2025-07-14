

- AppKit
- NSControlTextEditingDelegate
-  control(\_:textShouldEndEditing:) 

Instance Method

# control(\_:textShouldEndEditing:)

Invoked when the insertion point tries to leave a cell of the control that has been edited.

macOS

``` source
@MainActor
optional func control(
    _ control: NSControl,
    textShouldEndEditing fieldEditor: NSText
) -> Bool
```

## Parameters 

`control`  

The control for which editing is about to end.

`fieldEditor`  

The field editor of the control. You can use this parameter to get the edited text.

## Return Value

true if the insertion point should be allowed to end the editing session; otherwise, false.

## Discussion

This message is sent only by controls that allow editing of text (such as a text field or a form field). This message is sent by the control directly to its delegate object.

## See Also

### Responding to Text Editing

func control(NSControl, textShouldBeginEditing: NSText) -> Bool

Invoked when the user tries to enter a character in a cell of a control that allows editing of text (such as a text field or form field).

