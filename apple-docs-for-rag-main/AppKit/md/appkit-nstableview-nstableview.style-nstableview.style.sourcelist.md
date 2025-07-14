

- AppKit
- NSTableView
- NSTableView.Style
-  NSTableView.Style.sourceList 

Case

# NSTableView.Style.sourceList

The table view style resolves to a source-list style.

macOS 11.0+

``` source
case sourceList
```

## Discussion

A source-list style table adopts the standard metrics, row selection style, and background of a sidebar source list. In addition, an NSOutlineView with the source-list style adopts standard values for its indentationPerLevel, rowHeight, and intercellSpacing properties.

## See Also

### Table Styles

case automatic

The system resolves the table view style based on the table view hierarchy.

case fullWidth

The table view style resolves to a full-width style.

case inset

The table view style resolves to an inset style.

case plain

The table view style resolves to a plain style.

