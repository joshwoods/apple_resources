

- AppKit
- NSComboBox
-  willDismissNotification 

Type Property

# willDismissNotification

Posted whenever the pop-up list of the `NSComboBox` is about to be dismissed.

macOS

``` source
class let willDismissNotification: NSNotification.Name
```

## Discussion

The notification object is the `NSComboBox` whose pop-up list will be dismissed. This notification does not contain a `userInfo` dictionary.

## See Also

### Notifications

class let selectionDidChangeNotification: NSNotification.Name

Posted after the pop-up list selection of the `NSComboBox` changes.

class let selectionIsChangingNotification: NSNotification.Name

Posted whenever the pop-up list selection of the `NSComboBox` is changing.

class let willPopUpNotification: NSNotification.Name

Posted whenever the pop-up list of the `NSComboBox` is going to be displayed.

