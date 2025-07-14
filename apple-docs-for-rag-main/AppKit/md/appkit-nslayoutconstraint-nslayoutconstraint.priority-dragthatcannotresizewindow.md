

- AppKit
- NSLayoutConstraint
- NSLayoutConstraint.Priority
-  dragThatCannotResizeWindow 

Type Property

# dragThatCannotResizeWindow

Priority level at which a split view divider, say, is dragged.

macOS 10.7+

``` source
static let dragThatCannotResizeWindow: NSLayoutConstraint.Priority
```

## Discussion

A constraint with this priority cannot resize the window.

## See Also

### Constants

static let required: NSLayoutConstraint.Priority

A required constraint.

static let defaultHigh: NSLayoutConstraint.Priority

Priority level with which a button resists compressing its content.

static let dragThatCanResizeWindow: NSLayoutConstraint.Priority

Appropriate priority level for a drag that may end up resizing the window.

static let windowSizeStayPut: NSLayoutConstraint.Priority

Priority level for the window’s current size.

static let defaultLow: NSLayoutConstraint.Priority

Priority level at which a button hugs its contents horizontally.

static let fittingSizeCompression: NSLayoutConstraint.Priority

When you send a fittingSize message to a view, the smallest size that is large enough for the view’s contents is computed.

