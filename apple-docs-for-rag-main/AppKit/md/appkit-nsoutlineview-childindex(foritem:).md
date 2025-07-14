

- AppKit
- NSOutlineView
-  childIndex(forItem:) 

Instance Method

# childIndex(forItem:)

Returns the child index of the specified item within its parent.

macOS 10.11+

``` source
@MainActor
func childIndex(forItem item: Any) -> Int
```

## Discussion

The performance of this method is O(1) at best and O(n) at worst.

## See Also

### Getting Related Items

func parent(forItem: Any?) -> Any?

Returns the parent for a given item.

func child(Int, ofItem: Any?) -> Any?

Returns the specified child of an item.

func numberOfChildren(ofItem: Any?) -> Int

Returns the number of children for the specified parent item.

