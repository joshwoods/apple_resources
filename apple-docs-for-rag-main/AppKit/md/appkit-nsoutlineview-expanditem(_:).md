

- AppKit
- NSOutlineView
-  expandItem(\_:) 

Instance Method

# expandItem(\_:)

Expands a given item.

macOS

``` source
@MainActor
func expandItem(_ item: Any?)
```

## Parameters 

`item`  

An item in the receiver.

## Discussion

If `item` is not expandable or is already expanded, does nothing.

If expanding takes place, posts an item expanded notification.

## See Also

### Expanding and Collapsing the Outline

func expandItem(Any?, expandChildren: Bool)

Expands a specified item and, optionally, its children.

func collapseItem(Any?)

Collapses a given item.

func collapseItem(Any?, collapseChildren: Bool)

Collapses a given item and, optionally, its children.

