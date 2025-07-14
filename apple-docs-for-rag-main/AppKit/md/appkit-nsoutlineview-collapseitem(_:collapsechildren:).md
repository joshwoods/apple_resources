

- AppKit
- NSOutlineView
-  collapseItem(\_:collapseChildren:) 

Instance Method

# collapseItem(\_:collapseChildren:)

Collapses a given item and, optionally, its children.

macOS

``` source
@MainActor
func collapseItem(
    _ item: Any?,
    collapseChildren: Bool
)
```

## Parameters 

`item`  

An item in the receiver.

Starting in OS X version 10.5, passing `'nil'` will collapse each item under the root in the outline view.

`collapseChildren`  

If true, recursively collapses `item` and its children. If false, collapses `item` only (identical to collapseItem(_:)).

## Discussion

For example, this method is invoked with the `collapseChildren` parameter set to true when a user Option-clicks the disclosure triangle for an item in the outline view (to collapse the item and all its contained items).

For each item collapsed, posts an item collapsed notification.

## See Also

### Expanding and Collapsing the Outline

func expandItem(Any?)

Expands a given item.

func expandItem(Any?, expandChildren: Bool)

Expands a specified item and, optionally, its children.

func collapseItem(Any?)

Collapses a given item.

