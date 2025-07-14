

- AppKit
- NSTableRowView
-  draggingDestinationFeedbackStyle 

Instance Property

# draggingDestinationFeedbackStyle

Specifies the dragging destination feedback style.

macOS 10.7+

``` source
@MainActor
var draggingDestinationFeedbackStyle: NSTableView.DraggingDestinationFeedbackStyle { get set }
```

## Discussion

Possible values are defined in NSTableView.DraggingDestinationFeedbackStyle.

## See Also

### Drag and Drop

var indentationForDropOperation: CGFloat

Defines the amount the drag target for a row should be indented.

var isTargetForDropOperation: Bool

Specifies whether this row will draw a drop indicator based on the current dragging feedback style.

