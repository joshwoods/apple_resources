

- AppKit
- NSComboBoxDelegate
-  comboBoxSelectionDidChange(\_:) 

Instance Method

# comboBoxSelectionDidChange(\_:)

Informs the delegate that the pop-up list selection has finished changing.

macOS 10.10+

``` source
@MainActor
optional func comboBoxSelectionDidChange(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named selectionDidChangeNotification.

## See Also

### Related Documentation

Combo Box Programming Topics

### Manipulating the selection

func comboBoxSelectionIsChanging(Notification)

Informs the delegate that the pop-up list selection is changing.

func comboBoxWillDismiss(Notification)

Informs the delegate that the pop-up list is about to be dismissed.

func comboBoxWillPopUp(Notification)

Informs the delegate that the pop-up list is about to be displayed.

