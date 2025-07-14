

- AppKit
- NSTableRowView
-  indentationForDropOperation 

Instance Property

# indentationForDropOperation

Defines the amount the drag target for a row should be indented.

macOS 10.7+

``` source
@MainActor
var indentationForDropOperation: CGFloat { get set }
```

## Discussion

The default is `0`.

## See Also

### Drag and Drop

var draggingDestinationFeedbackStyle: NSTableView.DraggingDestinationFeedbackStyle

Specifies the dragging destination feedback style.

var isTargetForDropOperation: Bool

Specifies whether this row will draw a drop indicator based on the current dragging feedback style.

