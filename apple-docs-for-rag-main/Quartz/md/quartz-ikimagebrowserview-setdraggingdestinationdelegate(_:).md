

- Quartz
- IKImageBrowserView
-  setDraggingDestinationDelegate(\_:) 

Instance Method

# setDraggingDestinationDelegate(\_:)

Sets the dragging destination delegate of the receiver.

macOS 10.4+

``` source
@MainActor
func setDraggingDestinationDelegate(_ delegate: Any!)
```

## Parameters 

`delegate`  

The delegate (NSDraggingDestination) to set.

## See Also

### Supporting Drag and Drop

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

func dropOperation() -> IKImageBrowserDropOperation

Returns the current drop operation.

