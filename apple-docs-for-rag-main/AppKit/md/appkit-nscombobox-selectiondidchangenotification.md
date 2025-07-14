

- AppKit
- NSComboBox
-  selectionDidChangeNotification 

Type Property

# selectionDidChangeNotification

Posted after the pop-up list selection of the `NSComboBox` changes.

macOS

``` source
class let selectionDidChangeNotification: NSNotification.Name
```

## Discussion

The notification object is the `NSComboBox` whose selection changed. This notification does not contain a `userInfo` dictionary.

## See Also

### Notifications

class let selectionIsChangingNotification: NSNotification.Name

Posted whenever the pop-up list selection of the `NSComboBox` is changing.

class let willDismissNotification: NSNotification.Name

Posted whenever the pop-up list of the `NSComboBox` is about to be dismissed.

class let willPopUpNotification: NSNotification.Name

Posted whenever the pop-up list of the `NSComboBox` is going to be displayed.

