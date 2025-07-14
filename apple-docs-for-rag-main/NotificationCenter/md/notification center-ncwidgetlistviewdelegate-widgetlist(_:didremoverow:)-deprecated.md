

- Notification Center
- NCWidgetListViewDelegate
-  widgetList(\_:didRemoveRow:) Deprecated

Instance Method

# widgetList(\_:didRemoveRow:)

Tells the delegate that the specified row was removed from the list.

macOS 10.10–11.0Deprecated

``` source
optional func widgetList(
    _ list: NCWidgetListViewController,
    didRemoveRow row: Int
)
```

Deprecated

Use WidgetKit instead.

## Parameters 

`list`  

The widget’s list view controller.

`row`  

The row that was removed.

## Discussion

List item deletion is not enabled unless the delegate implements this method and widgetList(_:shouldRemoveRow:). The item represented by `row` is removed from the list view controller’s contents array before this method is called.

## See Also

### Adding and Deleting Rows

func widgetList(NCWidgetListViewController, shouldRemoveRow: Int) -> Bool

Asks the delegate to allow or prohibit the specified row to be removed from the list.

Deprecated

func widgetListPerformAddAction(NCWidgetListViewController)

Asks the delegate to perform an action when the Add (+) button is clicked.

Deprecated

