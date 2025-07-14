

- Quartz
- IKImageBrowserView
-  draggingDestinationDelegate() 

Instance Method

# draggingDestinationDelegate()

Returns the dragging destination delegate of the receiver.

macOS 10.4+

``` source
@MainActor
func draggingDestinationDelegate() -> Any!
```

## Return Value

The receiver’s dragging destination delegate.

## See Also

### Supporting Drag and Drop

func setDraggingDestinationDelegate(Any!)

Sets the dragging destination delegate of the receiver.

func setDrop(Int, dropOperation: IKImageBrowserDropOperation)

Allows the class to retarget the drop action.

func indexAtLocationOfDroppedItem() -> Int

Returns the index of the cell where the drop operation occurred.

func setAllowsDroppingOnItems(Bool)

Specifies whether the user can drop on items.

func allowsDroppingOnItems() -> Bool

Returns whether the user can drop on items.

func dropOperation() -> IKImageBrowserDropOperation

Returns the current drop operation.

