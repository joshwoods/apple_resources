

- AppKit
- NSOutlineView
-  columnDidMoveNotification 

Type Property

# columnDidMoveNotification

Posted whenever a column is moved by user action in an `NSOutlineView` object.

macOS

``` source
class let columnDidMoveNotification: NSNotification.Name
```

## Discussion

The notification object is the `NSOutlineView` object in which a column moved. The `userInfo` dictionary contains the following information:

| Key | Value |
|----|----|
| `@"NSOldColumn"` | An NSNumber object containing the integer value of the column’s original index |
| `@"NSNewColumn"` | An NSNumber object containing the integer value of the column’s present index |

## See Also

### Related Documentation

func moveColumn(Int, toColumn: Int)

Moves the column and heading at the specified index to the new specified index.

### Notifications

class let columnDidResizeNotification: NSNotification.Name

Posted whenever a column is resized in an `NSOutlineView` object.

class let itemDidCollapseNotification: NSNotification.Name

Posted whenever an item is collapsed in an `NSOutlineView` object.

class let itemDidExpandNotification: NSNotification.Name

Posted whenever an item is expanded in an `NSOutlineView` object.

class let itemWillCollapseNotification: NSNotification.Name

Posted before an item is collapsed (after the user clicks the arrow but before the item is collapsed).

class let itemWillExpandNotification: NSNotification.Name

Posted before an item is expanded (after the user clicks the arrow but before the item is collapsed).

class let selectionDidChangeNotification: NSNotification.Name

Posted after the outline view’s selection changes.

class let selectionIsChangingNotification: NSNotification.Name

Posted as the outline view’s selection changes (while the mouse button is still down).

