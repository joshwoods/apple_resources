

- AppKit
- NSLayoutConstraint
- NSLayoutConstraint.Priority
-  required 

Type Property

# required

A required constraint.

macOS 10.7+

``` source
static let required: NSLayoutConstraint.Priority
```

## Discussion

Do not specify a layout constraint that exceeds this number.

## See Also

### Constants

static let defaultHigh: NSLayoutConstraint.Priority

Priority level with which a button resists compressing its content.

static let dragThatCanResizeWindow: NSLayoutConstraint.Priority

Appropriate priority level for a drag that may end up resizing the window.

static let windowSizeStayPut: NSLayoutConstraint.Priority

Priority level for the window’s current size.

static let dragThatCannotResizeWindow: NSLayoutConstraint.Priority

Priority level at which a split view divider, say, is dragged.

static let defaultLow: NSLayoutConstraint.Priority

Priority level at which a button hugs its contents horizontally.

static let fittingSizeCompression: NSLayoutConstraint.Priority

When you send a fittingSize message to a view, the smallest size that is large enough for the view’s contents is computed.

