

- AppKit
- NSTableView
-  selectionIsChangingNotification 

Type Property

# selectionIsChangingNotification

Posted as an `NSTableView` object’s selection changes (while the mouse button is still down).

macOS

``` source
class let selectionIsChangingNotification: NSNotification.Name
```

## Discussion

Note that the notification is sent only for mouse events that change the table’s selection, not keyboard events. The notification object is the table view whose selection is changing. This notification does not contain a `userInfo` dictionary.

## See Also

### Notifications

class let columnDidMoveNotification: NSNotification.Name

Posted whenever a column is moved by user action in an `NSTableView` object.

class let columnDidResizeNotification: NSNotification.Name

Posted whenever a column is resized in an `NSTableView` object.

class let selectionDidChangeNotification: NSNotification.Name

Posted after an `NSTableView` object’s selection changes.

