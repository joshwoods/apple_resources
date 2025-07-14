

- AppKit
- NSOutlineView
-  level(forItem:) 

Instance Method

# level(forItem:)

Returns the indentation level for a given item.

macOS

``` source
@MainActor
func level(forItem item: Any?) -> Int
```

## Parameters 

`item`  

An item in the receiver.

## Return Value

The indentation level for `item`. If `item` is `nil` (which is the root item), returns `–1`.

## Discussion

The levels are zero-based—that is, the first level of displayed items is level `0`.

## See Also

### Working with Indentation

func level(forRow: Int) -> Int

Returns the indentation level for a given row.

var indentationPerLevel: CGFloat

The per-level indentation, measured in points.

var indentationMarkerFollowsCell: Bool

A Boolean value indicating whether the indentation marker symbol displayed in the outline column should be indented along with the cell contents.

