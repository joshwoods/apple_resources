

- AppKit
- NSTableRowView
-  isTargetForDropOperation 

Instance Property

# isTargetForDropOperation

Specifies whether this row will draw a drop indicator based on the current dragging feedback style.

macOS 10.7+

``` source
@MainActor
var isTargetForDropOperation: Bool { get set }
```

## Discussion

When true, the row view will draw a drop on indicator based on the current draggingDestinationFeedbackStyle.

## See Also

### Drag and Drop

var draggingDestinationFeedbackStyle: NSTableView.DraggingDestinationFeedbackStyle

Specifies the dragging destination feedback style.

var indentationForDropOperation: CGFloat

Defines the amount the drag target for a row should be indented.

