

- AppKit
- NSOutlineView
-  expandItem(\_:expandChildren:) 

Instance Method

# expandItem(\_:expandChildren:)

Expands a specified item and, optionally, its children.

macOS

``` source
@MainActor
func expandItem(
    _ item: Any?,
    expandChildren: Bool
)
```

## Parameters 

`item`  

An item in the receiver.

Starting in OS X version 10.5, passing `'nil'` will expand each item under the root in the outline view.

`expandChildren`  

If true, recursively expands `item` and its children. If false, expands `item` only (identical to expandItem(_:)).

## Discussion

For example, this method is invoked with the `expandChildren` parameter set to true when a user Option-clicks the disclosure triangle for an item in the outline view (to expand the item and all its contained items).

For each item expanded, posts an item expanded notification.

## See Also

### Expanding and Collapsing the Outline

func expandItem(Any?)

Expands a given item.

func collapseItem(Any?)

Collapses a given item.

func collapseItem(Any?, collapseChildren: Bool)

Collapses a given item and, optionally, its children.

