

- AppKit
- NSLayoutConstraint
- NSLayoutConstraint.Priority
-  windowSizeStayPut 

Type Property

# windowSizeStayPut

Priority level for the window’s current size.

macOS 10.7+

``` source
static let windowSizeStayPut: NSLayoutConstraint.Priority
```

## Discussion

It’s generally not appropriate to make a constraint at exactly this priority. You want to be higher or lower. Constraints with higher priorities can adjust the window’s size. Constraints with lower priorities must be fulfilled using the current window size.

## See Also

### Constants

static let required: NSLayoutConstraint.Priority

A required constraint.

static let defaultHigh: NSLayoutConstraint.Priority

Priority level with which a button resists compressing its content.

static let dragThatCanResizeWindow: NSLayoutConstraint.Priority

Appropriate priority level for a drag that may end up resizing the window.

static let dragThatCannotResizeWindow: NSLayoutConstraint.Priority

Priority level at which a split view divider, say, is dragged.

static let defaultLow: NSLayoutConstraint.Priority

Priority level at which a button hugs its contents horizontally.

static let fittingSizeCompression: NSLayoutConstraint.Priority

When you send a fittingSize message to a view, the smallest size that is large enough for the view’s contents is computed.

