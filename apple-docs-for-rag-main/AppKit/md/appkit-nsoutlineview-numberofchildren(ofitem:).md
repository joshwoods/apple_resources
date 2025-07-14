

- AppKit
- NSOutlineView
-  numberOfChildren(ofItem:) 

Instance Method

# numberOfChildren(ofItem:)

Returns the number of children for the specified parent item.

macOS 10.10+

``` source
@MainActor
func numberOfChildren(ofItem item: Any?) -> Int
```

## Parameters 

`item`  

The parent item.

## Return Value

The number of children associated with the parent.

## Discussion

You can call this method on an outline view with either a static or dynamic data source. For an outline view whose contents are dynamic, this method may call out to the outlineView(_:numberOfChildrenOfItem:) method of the associated data source object.

## See Also

### Getting Related Items

func parent(forItem: Any?) -> Any?

Returns the parent for a given item.

func childIndex(forItem: Any) -> Int

Returns the child index of the specified item within its parent.

func child(Int, ofItem: Any?) -> Any?

Returns the specified child of an item.

