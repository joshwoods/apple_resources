

- AppKit
- NSComboBox
-  selectionIsChangingNotification 

Type Property

# selectionIsChangingNotification

Posted whenever the pop-up list selection of the `NSComboBox` is changing.

macOS

``` source
class let selectionIsChangingNotification: NSNotification.Name
```

## Discussion

The notification object is the `NSComboBox` whose selection is changing. This notification does not contain a `userInfo` dictionary.

## See Also

### Notifications

class let selectionDidChangeNotification: NSNotification.Name

Posted after the pop-up list selection of the `NSComboBox` changes.

class let willDismissNotification: NSNotification.Name

Posted whenever the pop-up list of the `NSComboBox` is about to be dismissed.

class let willPopUpNotification: NSNotification.Name

Posted whenever the pop-up list of the `NSComboBox` is going to be displayed.

