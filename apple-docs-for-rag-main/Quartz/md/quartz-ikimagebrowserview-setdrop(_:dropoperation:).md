

- Quartz
- IKImageBrowserView
-  setDrop(\_:dropOperation:) 

Instance Method

# setDrop(\_:dropOperation:)

Allows the class to retarget the drop action.

macOS 10.4+

``` source
@MainActor
func setDrop(
    _ index: Int,
    dropOperation operation: IKImageBrowserDropOperation
)
```

## Parameters 

`index`  

The requested drop index.

`operation`  

The requested drop operation. The possible values are described in IKImageBrowserDropOperation.

## Discussion

For example, To specify a drop on the second item, one would specify index as `1`, and operation as IKImageBrowserDropOn. To specify a drop after the last item, one would specify index as the number of items and operation as IKImageBrowserDropBefore.

Passing a value of `–1` for `index`, and IKImageBrowserDropOn as the operation causes the entire browser view to be highlighted rather than a specific item. This is useful if the data displayed by the receiver does not allow the user to drop items at a specific item location

.

## See Also

### Supporting Drag and Drop

func setDraggingDestinationDelegate(Any!)

Sets the dragging destination delegate of the receiver.

func draggingDestinationDelegate() -> Any!

Returns the dragging destination delegate of the receiver.

func indexAtLocationOfDroppedItem() -> Int

Returns the index of the cell where the drop operation occurred.

func setAllowsDroppingOnItems(Bool)

Specifies whether the user can drop on items.

func allowsDroppingOnItems() -> Bool

Returns whether the user can drop on items.

func dropOperation() -> IKImageBrowserDropOperation

Returns the current drop operation.

