

- Notification Center
- NCWidgetListViewDelegate
-  widgetList(\_:shouldRemoveRow:) Deprecated

Instance Method

# widgetList(\_:shouldRemoveRow:)

Asks the delegate to allow or prohibit the specified row to be removed from the list.

macOS 10.10–11.0Deprecated

``` source
optional func widgetList(
    _ list: NCWidgetListViewController,
    shouldRemoveRow row: Int
) -> Bool
```

Deprecated

Use WidgetKit instead.

## Parameters 

`list`  

The widget’s list view controller.

`row`  

The row that should be removed.

## Return Value

true if the specified row can be removed, otherwise false.

## Discussion

List item deletion is not enabled unless the delegate implements this method and widgetList(_:didRemoveRow:). Returning false prohibits `row` from being deleted. Returning YES allows `row` to be deleted, and the delegate will be called again when the item that `row` represents is deleted from the list view controller’s contents array.

## See Also

### Adding and Deleting Rows

func widgetList(NCWidgetListViewController, didRemoveRow: Int)

Tells the delegate that the specified row was removed from the list.

Deprecated

func widgetListPerformAddAction(NCWidgetListViewController)

Asks the delegate to perform an action when the Add (+) button is clicked.

Deprecated

