

- AppKit
- NSOutlineView
-  reloadItem(\_:reloadChildren:) 

Instance Method

# reloadItem(\_:reloadChildren:)

Reloads a given item and, optionally, its children.

macOS

``` source
@MainActor
func reloadItem(
    _ item: Any?,
    reloadChildren: Bool
)
```

## Parameters 

`item`  

An item in the receiver.

Starting in OS X version 10.5, passing `'nil'` will reload everything under the root in the outline view.

`reloadChildren`  

If true, recursively reloads `item` and its children. If false, reloads `item` only (identical to reloadItem(_:)).

It is not necessary, or efficient, to reload children if the item is not expanded.

## See Also

### Redisplaying Information

func reloadItem(Any?)

Reloads and redisplays the data for the given item.

