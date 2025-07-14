

- Quartz
- IKImageBrowserView
-  setAllowsDroppingOnItems(\_:) 

Instance Method

# setAllowsDroppingOnItems(\_:)

Specifies whether the user can drop on items.

macOS 10.4+

``` source
@MainActor
func setAllowsDroppingOnItems(_ flag: Bool)
```

## Parameters 

`flag`  

true if the user is able to drop on items, otherwise false.

## Discussion

The default is false.

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

func allowsDroppingOnItems() -> Bool

Returns whether the user can drop on items.

func dropOperation() -> IKImageBrowserDropOperation

Returns the current drop operation.

