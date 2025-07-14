

- AppKit
- NSOutlineView
-  indentationMarkerFollowsCell 

Instance Property

# indentationMarkerFollowsCell

A Boolean value indicating whether the indentation marker symbol displayed in the outline column should be indented along with the cell contents.

macOS

``` source
@MainActor
var indentationMarkerFollowsCell: Bool { get set }
```

## Discussion

When the value of this property is true, the indentation marker is indented along with the cell contents. When the value is false, the marker is always displayed left-justified in the column. The default value of this property is true.

## See Also

### Working with Indentation

func level(forItem: Any?) -> Int

Returns the indentation level for a given item.

func level(forRow: Int) -> Int

Returns the indentation level for a given row.

var indentationPerLevel: CGFloat

The per-level indentation, measured in points.

