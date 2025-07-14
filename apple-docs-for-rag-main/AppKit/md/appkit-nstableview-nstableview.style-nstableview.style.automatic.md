

- AppKit
- NSTableView
- NSTableView.Style
-  NSTableView.Style.automatic 

Case

# NSTableView.Style.automatic

The system resolves the table view style based on the table view hierarchy.

macOS 11.0+

``` source
case automatic
```

## Discussion

The system resolves the table view style in the following manner:

- If the table view is in a sidebar split-view controller item, effectiveStyle resolves to NSTableView.Style.sourceList.

- If the table’s scroll view has a border, effectiveStyle resolves to NSTableView.Style.fullWidth.

- Otherwise, effectiveStyle resolves to NSTableView.Style.inset. However, if the table needs extra space to fit its column cells, effectiveStyle resolves to NSTableView.Style.fullWidth.

Note

For backward compatibility reasons, when selectionHighlightStyle is NSTableView.SelectionHighlightStyle.sourceList, style also resolves to NSTableView.Style.sourceList.

## See Also

### Table Styles

case fullWidth

The table view style resolves to a full-width style.

case inset

The table view style resolves to an inset style.

case sourceList

The table view style resolves to a source-list style.

case plain

The table view style resolves to a plain style.

