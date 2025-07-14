

- AppKit
-  NSComboBoxDelegate 

Protocol

# NSComboBoxDelegate

A set of optional methods implemented by delegates of combo box objects.

macOS

``` source
protocol NSComboBoxDelegate : NSTextFieldDelegate
```

## Topics

### Manipulating the selection

func comboBoxSelectionDidChange(Notification)

Informs the delegate that the pop-up list selection has finished changing.

func comboBoxSelectionIsChanging(Notification)

Informs the delegate that the pop-up list selection is changing.

func comboBoxWillDismiss(Notification)

Informs the delegate that the pop-up list is about to be dismissed.

func comboBoxWillPopUp(Notification)

Informs the delegate that the pop-up list is about to be displayed.

## Relationships

### Inherits From

- NSControlTextEditingDelegate
- NSObjectProtocol
- NSTextFieldDelegate

## See Also

### Management

protocol NSComboBoxDataSource

