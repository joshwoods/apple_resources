

- AppKit
- NSTableView
-  selectionDidChangeNotification 

Type Property

# selectionDidChangeNotification

Posted after an `NSTableView` object’s selection changes.

macOS

``` source
class let selectionDidChangeNotification: NSNotification.Name
```

## Discussion

The notification object is the table view whose selection changed. This notification does not contain a `userInfo` dictionary.

## See Also

### Notifications

class let columnDidMoveNotification: NSNotification.Name

Posted whenever a column is moved by user action in an `NSTableView` object.

class let columnDidResizeNotification: NSNotification.Name

Posted whenever a column is resized in an `NSTableView` object.

class let selectionIsChangingNotification: NSNotification.Name

Posted as an `NSTableView` object’s selection changes (while the mouse button is still down).

