

- AppKit
- NSLayoutConstraint
- NSLayoutConstraint.Priority
-  dragThatCanResizeWindow 

Type Property

# dragThatCanResizeWindow

Appropriate priority level for a drag that may end up resizing the window.

macOS 10.7+

``` source
static let dragThatCanResizeWindow: NSLayoutConstraint.Priority
```

## Discussion

This drag does not need to explicitly resize the window. The user might be dragging around window contents, and it might be desirable for the window get bigger to accommodate those contents.

## See Also

### Constants

static let required: NSLayoutConstraint.Priority

A required constraint.

static let defaultHigh: NSLayoutConstraint.Priority

Priority level with which a button resists compressing its content.

static let windowSizeStayPut: NSLayoutConstraint.Priority

Priority level for the window’s current size.

static let dragThatCannotResizeWindow: NSLayoutConstraint.Priority

Priority level at which a split view divider, say, is dragged.

static let defaultLow: NSLayoutConstraint.Priority

Priority level at which a button hugs its contents horizontally.

static let fittingSizeCompression: NSLayoutConstraint.Priority

When you send a fittingSize message to a view, the smallest size that is large enough for the view’s contents is computed.

