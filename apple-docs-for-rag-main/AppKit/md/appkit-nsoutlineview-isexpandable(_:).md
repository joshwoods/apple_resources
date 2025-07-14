

- AppKit
- NSOutlineView
-  isExpandable(\_:) 

Instance Method

# isExpandable(\_:)

Returns a Boolean value that indicates whether a given item is expandable.

macOS

``` source
@MainActor
func isExpandable(_ item: Any?) -> Bool
```

## Parameters 

`item`  

An item in the receiver.

## Return Value

true if `item` is expandable—that is, `item` can contain other items, otherwise false.

## See Also

### Related Documentation

func expandItem(Any?)

Expands a given item.

### Working with Expandability

func isItemExpanded(Any?) -> Bool

Returns a Boolean value that indicates whether a given item is expanded.

