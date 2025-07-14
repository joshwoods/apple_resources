

- AppKit
- NSOutlineView
-  parent(forItem:) 

Instance Method

# parent(forItem:)

Returns the parent for a given item.

macOS

``` source
@MainActor
func parent(forItem item: Any?) -> Any?
```

## Parameters 

`item`  

The item for which to return the parent.

## Return Value

The parent for `item`, or `nil` if the parent is the root.

## See Also

### Getting Related Items

func childIndex(forItem: Any) -> Int

Returns the child index of the specified item within its parent.

func child(Int, ofItem: Any?) -> Any?

Returns the specified child of an item.

func numberOfChildren(ofItem: Any?) -> Int

Returns the number of children for the specified parent item.

