

- AppKit
- NSOutlineView
-  collapseItem(\_:) 

Instance Method

# collapseItem(\_:)

Collapses a given item.

macOS

``` source
@MainActor
func collapseItem(_ item: Any?)
```

## Parameters 

`item`  

An item in the receiver.

## Discussion

If `item` is not expanded or not expandable, does nothing

If collapsing takes place, posts item collapse notification.

## See Also

### Expanding and Collapsing the Outline

func expandItem(Any?)

Expands a given item.

func expandItem(Any?, expandChildren: Bool)

Expands a specified item and, optionally, its children.

func collapseItem(Any?, collapseChildren: Bool)

Collapses a given item and, optionally, its children.

