

- Notification Center
- NCWidgetListViewDelegate
-  widgetList(\_:shouldReorderRow:) Deprecated

Instance Method

# widgetList(\_:shouldReorderRow:)

Asks the delegate to allow or prohibit the specified row to be moved to a new location in the list.

macOS 10.10–11.0Deprecated

``` source
optional func widgetList(
    _ list: NCWidgetListViewController,
    shouldReorderRow row: Int
) -> Bool
```

Deprecated

Use WidgetKit instead.

## Parameters 

`list`  

The widget’s list view controller.

`row`  

The row that should be moved.

## Return Value

true if specified row can be moved, otherwise false.

## Discussion

List item reordering is not enabled unless the delegate implements this method and widgetList(_:didReorderRow:toRow:). Returning false prohibits `row` from being moved. Returning YES allows `row` to be moved, and the delegate will be called again when the item that `row` represents is relocated in the list view controller’s contents array.

## See Also

### Reordering List Rows

func widgetList(NCWidgetListViewController, didReorderRow: Int, toRow: Int)

Tells the delegate that the specified row was moved to a new location.

Deprecated

