

- Quartz
- IKImageBrowserView
-  dropOperation() 

Instance Method

# dropOperation()

Returns the current drop operation.

macOS 10.4+

``` source
@MainActor
func dropOperation() -> IKImageBrowserDropOperation
```

## Return Value

IKImageBrowserDropOn if the drop occurs on an item, otherwise IKImageBrowserDropBefore.

## Discussion

The returned value is valid when a drop occurred and until next drop.

For example, given a browser with `N` cells , a cell of `N-1` and operation of IKImageBrowserDropOn would specify a drop on the last cell. To specify a drop after the last cell, one would use an index of `N` and IKImageBrowserDropBefore for the operation.

## See Also

### Supporting Drag and Drop

func setDraggingDestinationDelegate(Any!)

Sets the dragging destination delegate of the receiver.

func draggingDestinationDelegate() -> Any!

Returns the dragging destination delegate of the receiver.

func setDrop(Int, dropOperation: IKImageBrowserDropOperation)

Allows the class to retarget the drop action.

func indexAtLocationOfDroppedItem() -> Int

Returns the index of the cell where the drop operation occurred.

func setAllowsDroppingOnItems(Bool)

Specifies whether the user can drop on items.

func allowsDroppingOnItems() -> Bool

Returns whether the user can drop on items.

