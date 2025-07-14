

- AppKit
- NSOutlineView
-  indentationPerLevel 

Instance Property

# indentationPerLevel

The per-level indentation, measured in points.

macOS

``` source
@MainActor
var indentationPerLevel: CGFloat { get set }
```

## See Also

### Working with Indentation

func level(forItem: Any?) -> Int

Returns the indentation level for a given item.

func level(forRow: Int) -> Int

Returns the indentation level for a given row.

var indentationMarkerFollowsCell: Bool

A Boolean value indicating whether the indentation marker symbol displayed in the outline column should be indented along with the cell contents.

