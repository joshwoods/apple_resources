

- AppKit
- NSOutlineView
-  setDropItem(\_:dropChildIndex:) 

Instance Method

# setDropItem(\_:dropChildIndex:)

Used to “retarget” a proposed drop.

macOS

``` source
@MainActor
func setDropItem(
    _ item: Any?,
    dropChildIndex index: Int
)
```

## Parameters 

`item`  

The target item.

`index`  

The drop index.

## Discussion

For example, to specify a drop on `someOutlineItem`, you specify `item` as `someOutlineItem` and `index` as NSOutlineViewDropOnItemIndex. To specify a drop between child `2` and `3` of `someOutlineItem`, you specify `item` as `someOutlineItem` and `index` as `3` (children are a zero-based index). To specify a drop on an un-expandable `someOutlineItem`, you specify `item` as `someOutlineItem` and `index` as NSOutlineViewDropOnItemIndex.

## See Also

### Supporting Drag and Drop

func shouldCollapseAutoExpandedItems(forDeposited: Bool) -> Bool

Returns a Boolean value that indicates whether auto-expanded items should return to their original collapsed state.

