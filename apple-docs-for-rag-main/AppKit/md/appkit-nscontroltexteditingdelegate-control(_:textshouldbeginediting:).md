

- AppKit
- NSControlTextEditingDelegate
-  control(\_:textShouldBeginEditing:) 

Instance Method

# control(\_:textShouldBeginEditing:)

Invoked when the user tries to enter a character in a cell of a control that allows editing of text (such as a text field or form field).

macOS

``` source
@MainActor
optional func control(
    _ control: NSControl,
    textShouldBeginEditing fieldEditor: NSText
) -> Bool
```

## Parameters 

`control`  

The control whose content is about to be edited.

`fieldEditor`  

The field editor of the control.

## Return Value

true if the control’s field editor should be allowed to start editing the text; otherwise, false.

## Discussion

You can use this method to allow or disallow editing in a control. This message is sent by the control directly to its delegate object.

## See Also

### Responding to Text Editing

func control(NSControl, textShouldEndEditing: NSText) -> Bool

Invoked when the insertion point tries to leave a cell of the control that has been edited.

