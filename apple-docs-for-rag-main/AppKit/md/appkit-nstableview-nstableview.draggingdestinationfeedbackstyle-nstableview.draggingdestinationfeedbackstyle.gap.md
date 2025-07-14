

- AppKit
- NSTableView
- NSTableView.DraggingDestinationFeedbackStyle
-  NSTableView.DraggingDestinationFeedbackStyle.gap 

Case

# NSTableView.DraggingDestinationFeedbackStyle.gap

Provides a gap insertion when dragging over the table. Note that this style is only officially supported for NSView-based table views, but may partially work in Cell Based TableViews. The decision to use the gap style (compared to another style) can be made in tableView(_:draggingSession:willBeginAt:forRowIndexes:), or it can dynamically be changed.

macOS 10.9+

``` source
case gap
```

## See Also

### Constants

case none

Provides no feedback when the user drags over the table view. This option exists to allow subclasses to implement their dragging destination highlighting, or to make it not show anything all.

case regular

Draws a solid round-rect background on drop target rows, and an insertion marker between rows. This style should be used in most cases.

case sourceList

Draws an outline on drop target rows, and an insertion marker between rows. This style will automatically be set for source lists when the table’s unhideRows(at:withAnimation:) is set to NSTableView.DraggingDestinationFeedbackStyle.sourceList. This is the standard look for Source Lists, but may be used in other areas as needed.

