

- AppKit
- NSTableView
- NSTableView.SelectionHighlightStyle
-  NSTableView.SelectionHighlightStyle.sourceList Deprecated

Case

# NSTableView.SelectionHighlightStyle.sourceList

macOS 10.5–12.0Deprecated

``` source
case sourceList
```

Deprecated

Set the NSTableView.style property to NSTableViewStyleSourceList instead.

## Discussion

The source list style of NSTableView. On 10.5, a light blue gradient is used to highlight selected rows.

Note

When using this style, cell subclasses that implement `drawsBackground` must set the value to false. Otherwise, the cells will draw over the tableview’s highlighting.

## See Also

### Constants

case none

case regular

