

- AppKit
- NSComboBoxDelegate
-  comboBoxWillDismiss(\_:) 

Instance Method

# comboBoxWillDismiss(\_:)

Informs the delegate that the pop-up list is about to be dismissed.

macOS 10.10+

``` source
@MainActor
optional func comboBoxWillDismiss(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named willDismissNotification.

## See Also

### Manipulating the selection

func comboBoxSelectionDidChange(Notification)

Informs the delegate that the pop-up list selection has finished changing.

func comboBoxSelectionIsChanging(Notification)

Informs the delegate that the pop-up list selection is changing.

func comboBoxWillPopUp(Notification)

Informs the delegate that the pop-up list is about to be displayed.

