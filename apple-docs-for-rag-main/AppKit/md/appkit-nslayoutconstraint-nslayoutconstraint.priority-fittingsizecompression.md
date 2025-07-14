

- AppKit
- NSLayoutConstraint
- NSLayoutConstraint.Priority
-  fittingSizeCompression 

Type Property

# fittingSizeCompression

When you send a fittingSize message to a view, the smallest size that is large enough for the view’s contents is computed.

macOS 10.7+

``` source
static let fittingSizeCompression: NSLayoutConstraint.Priority
```

## Discussion

This is the priority level with which the view wants to be as small as possible in that computation. It’s quite low. It is generally not appropriate to make a constraint at exactly this priority. You want to be higher or lower.

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

static let dragThatCannotResizeWindow: NSLayoutConstraint.Priority

Priority level at which a split view divider, say, is dragged.

static let defaultLow: NSLayoutConstraint.Priority

Priority level at which a button hugs its contents horizontally.

