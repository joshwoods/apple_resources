

- Notification Center
- NCWidgetListViewDelegate
-  widgetList(\_:didReorderRow:toRow:) Deprecated

Instance Method

# widgetList(\_:didReorderRow:toRow:)

Tells the delegate that the specified row was moved to a new location.

macOS 10.10–11.0Deprecated

``` source
optional func widgetList(
    _ list: NCWidgetListViewController,
    didReorderRow row: Int,
    toRow newIndex: Int
)
```

Deprecated

Use WidgetKit instead.

## Parameters 

`list`  

The widget’s list view controller.

`row`  

The row that was moved.

`newIndex`  

The new location of `row`.

## Discussion

List item reordering is not enabled unless the delegate implements this method and widgetList(_:shouldReorderRow:). The item represented by `row` is moved to its new location in the list view controller’s contents array before this method is called.

## See Also

### Reordering List Rows

func widgetList(NCWidgetListViewController, shouldReorderRow: Int) -> Bool

Asks the delegate to allow or prohibit the specified row to be moved to a new location in the list.

Deprecated

