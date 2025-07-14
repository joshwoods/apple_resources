

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:heightOfRowByItem:) 

Instance Method

# outlineView(\_:heightOfRowByItem:)

Returns the height in points of the row containing `item`.

macOS 10.0+

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    heightOfRowByItem item: Any
) -> CGFloat
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`item`  

The row item.

## Return Value

The height of the row.

## Discussion

Values returned by this method should not include intercell spacing and must be greater than `0`.

Implement this method to support an outline view with varying row heights.

For large tables in particular, you should make sure that this method is efficient. `NSOutlineView` may cache the values this method returns, so if you would like to change a row’s height make sure to invalidate the row height by calling noteHeightOfRows(withIndexesChanged:). `NSOutlineView` automatically invalidates its entire row height cache in reloadData() and noteNumberOfRowsChanged().

If you call view(atColumn:row:makeIfNecessary:) or rowView(atRow:makeIfNecessary:) within your implementation of this method, an exception is thrown.

Important

To avoid the possibility of a hang due to unexpected recursion, don’t call geometry-calculating methods such as bounds, rect(ofColumn:), or any `NSTableView` method that calls tile() within your implementation of this method.

## See Also

### Customizing Column and Row Sizes

func outlineView(NSOutlineView, sizeToFitWidthOfColumn: Int) -> CGFloat

Invoked to allow the delegate to provide custom sizing behavior when a column’s resize divider is double clicked.

