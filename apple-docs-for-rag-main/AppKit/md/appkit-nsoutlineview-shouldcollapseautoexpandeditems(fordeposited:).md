

- AppKit
- NSOutlineView
-  shouldCollapseAutoExpandedItems(forDeposited:) 

Instance Method

# shouldCollapseAutoExpandedItems(forDeposited:)

Returns a Boolean value that indicates whether auto-expanded items should return to their original collapsed state.

macOS

``` source
@MainActor
func shouldCollapseAutoExpandedItems(forDeposited deposited: Bool) -> Bool
```

## Parameters 

`deposited`  

If true, the drop terminated successfully; if false the drop failed.

## Return Value

true if auto-expanded items should return to their original collapsed state; otherwise false.

## Discussion

Override this method to provide custom behavior. If the target of a drop is not auto-expanded (by hovering long enough) the drop target still gets expanded after a successful drop unless this method returns true. The default implementation returns false after a successful drop.

This method is called in a variety of situations. For example, it is called shortly after the outlineView(_:acceptDrop:item:childIndex:) method is called and also if the drag exits the outline view (exiting the view is treated the same as a failed drop). The return value of the outlineView(_:acceptDrop:item:childIndex:) method determines the incoming value of the `deposited` parameter.

## See Also

### Supporting Drag and Drop

func setDropItem(Any?, dropChildIndex: Int)

Used to “retarget” a proposed drop.

