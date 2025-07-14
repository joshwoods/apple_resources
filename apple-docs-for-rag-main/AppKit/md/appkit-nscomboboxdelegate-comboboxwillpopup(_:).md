

- AppKit
- NSComboBoxDelegate
-  comboBoxWillPopUp(\_:) 

Instance Method

# comboBoxWillPopUp(\_:)

Informs the delegate that the pop-up list is about to be displayed.

macOS 10.10+

``` source
@MainActor
optional func comboBoxWillPopUp(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named willPopUpNotification.

## See Also

### Manipulating the selection

func comboBoxSelectionDidChange(Notification)

Informs the delegate that the pop-up list selection has finished changing.

func comboBoxSelectionIsChanging(Notification)

Informs the delegate that the pop-up list selection is changing.

func comboBoxWillDismiss(Notification)

Informs the delegate that the pop-up list is about to be dismissed.

