

- AppKit
- NSComboBox
-  willPopUpNotification 

Type Property

# willPopUpNotification

Posted whenever the pop-up list of the `NSComboBox` is going to be displayed.

macOS

``` source
class let willPopUpNotification: NSNotification.Name
```

## Discussion

The notification object is the `NSComboBox` whose pop-up window will be displayed. This notification does not contain a `userInfo` dictionary.

## See Also

### Notifications

class let selectionDidChangeNotification: NSNotification.Name

Posted after the pop-up list selection of the `NSComboBox` changes.

class let selectionIsChangingNotification: NSNotification.Name

Posted whenever the pop-up list selection of the `NSComboBox` is changing.

class let willDismissNotification: NSNotification.Name

Posted whenever the pop-up list of the `NSComboBox` is about to be dismissed.

