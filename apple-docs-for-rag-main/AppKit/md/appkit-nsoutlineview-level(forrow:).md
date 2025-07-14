

- AppKit
- NSOutlineView
-  level(forRow:) 

Instance Method

# level(forRow:)

Returns the indentation level for a given row.

macOS

``` source
@MainActor
func level(forRow row: Int) -> Int
```

## Parameters 

`row`  

The index of a row in the receiver.

## Return Value

The indentation level for `row`. For an invalid row, returns `–1`.

## Discussion

The levels are zero-based—that is, the first level of displayed items is level `0`.

## See Also

### Working with Indentation

func level(forItem: Any?) -> Int

Returns the indentation level for a given item.

var indentationPerLevel: CGFloat

The per-level indentation, measured in points.

var indentationMarkerFollowsCell: Bool

A Boolean value indicating whether the indentation marker symbol displayed in the outline column should be indented along with the cell contents.

