

- AppKit
- NSTableView
-  columnDidResizeNotification 

Type Property

# columnDidResizeNotification

Posted whenever a column is resized in an `NSTableView` object.

macOS

``` source
class let columnDidResizeNotification: NSNotification.Name
```

## Discussion

The notification object is the table view in which a column was resized. The `userInfo` dictionary contains the following information:

| Key | Value |
|----|----|
| `@"NSTableColumn"` | The column that was resized. |
| `@"NSOldWidth"` | An NSNumber containing the integer value of the column’s original width. |

## See Also

### Notifications

class let columnDidMoveNotification: NSNotification.Name

Posted whenever a column is moved by user action in an `NSTableView` object.

class let selectionDidChangeNotification: NSNotification.Name

Posted after an `NSTableView` object’s selection changes.

class let selectionIsChangingNotification: NSNotification.Name

Posted as an `NSTableView` object’s selection changes (while the mouse button is still down).

