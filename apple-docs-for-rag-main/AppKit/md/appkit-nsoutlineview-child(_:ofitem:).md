

- AppKit
- NSOutlineView
-  child(\_:ofItem:) 

Instance Method

# child(\_:ofItem:)

Returns the specified child of an item.

macOS 10.10+

``` source
@MainActor
func child(
    _ index: Int,
    ofItem item: Any?
) -> Any?
```

## Parameters 

`index`  

The index of the child item in the parent.

`item`  

The parent item whose child item you want to retrieve.

## Return Value

The child item or `nil` if the item could not be found.

## Discussion

You can call this method on an outline view with either a static or dynamic data source. For an outline view whose contents are dynamic, this method may call out to the outlineView(_:child:ofItem:) method of the associated data source object.

## See Also

### Getting Related Items

func parent(forItem: Any?) -> Any?

Returns the parent for a given item.

func childIndex(forItem: Any) -> Int

Returns the child index of the specified item within its parent.

func numberOfChildren(ofItem: Any?) -> Int

Returns the number of children for the specified parent item.

