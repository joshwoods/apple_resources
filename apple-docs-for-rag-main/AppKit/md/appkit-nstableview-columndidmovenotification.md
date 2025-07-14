

- AppKit
- NSTableView
-  columnDidMoveNotification 

Type Property

# columnDidMoveNotification

Posted whenever a column is moved by user action in an `NSTableView` object.

macOS

``` source
class let columnDidMoveNotification: NSNotification.Name
```

## Discussion

The notification object is the table view in which a column moved. The `userInfo` dictionary contains the following information:

| Key | Value |
|----|----|
| `@"NSOldColumn"` | An `NSNumber` object containing the integer value of the column’s original index. |
| `@"NSNewColumn"` | An `NSNumber` object containing the integer value of the column’s present index. |

## See Also

### Related Documentation

func moveColumn(Int, toColumn: Int)

Moves the column and heading at the specified index to the new specified index.

### Notifications

class let columnDidResizeNotification: NSNotification.Name

Posted whenever a column is resized in an `NSTableView` object.

class let selectionDidChangeNotification: NSNotification.Name

Posted after an `NSTableView` object’s selection changes.

class let selectionIsChangingNotification: NSNotification.Name

Posted as an `NSTableView` object’s selection changes (while the mouse button is still down).

