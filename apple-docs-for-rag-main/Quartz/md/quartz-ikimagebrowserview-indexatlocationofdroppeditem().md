

- Quartz
- IKImageBrowserView
-  indexAtLocationOfDroppedItem() 

Instance Method

# indexAtLocationOfDroppedItem()

Returns the index of the cell where the drop operation occurred.

macOS 10.4+

``` source
@MainActor
func indexAtLocationOfDroppedItem() -> Int
```

## Return Value

The index of the cell where the drop operation occurred.

## Discussion

The returned index is valid until the next drop occurs.

## See Also

### Supporting Drag and Drop

func setDraggingDestinationDelegate(Any!)

Sets the dragging destination delegate of the receiver.

func draggingDestinationDelegate() -> Any!

Returns the dragging destination delegate of the receiver.

func setDrop(Int, dropOperation: IKImageBrowserDropOperation)

Allows the class to retarget the drop action.

func setAllowsDroppingOnItems(Bool)

Specifies whether the user can drop on items.

func allowsDroppingOnItems() -> Bool

Returns whether the user can drop on items.

func dropOperation() -> IKImageBrowserDropOperation

Returns the current drop operation.

