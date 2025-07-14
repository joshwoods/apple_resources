

- AppKit
- NSComboBoxDelegate
-  comboBoxSelectionIsChanging(\_:) 

Instance Method

# comboBoxSelectionIsChanging(\_:)

Informs the delegate that the pop-up list selection is changing.

macOS 10.10+

``` source
@MainActor
optional func comboBoxSelectionIsChanging(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named selectionIsChangingNotification.

## See Also

### Manipulating the selection

func comboBoxSelectionDidChange(Notification)

Informs the delegate that the pop-up list selection has finished changing.

func comboBoxWillDismiss(Notification)

Informs the delegate that the pop-up list is about to be dismissed.

func comboBoxWillPopUp(Notification)

Informs the delegate that the pop-up list is about to be displayed.

