

- UIKit
- UILayoutPriority
-  fittingSizeLevel 

Type Property

# fittingSizeLevel

The priority level with which the view wants to conform to the target size in that computation.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
static let fittingSizeLevel: UILayoutPriority
```

## Discussion

When you send a systemLayoutSizeFitting(_:) message to a view, the size fitting most closely to the target size is computed. This priority is quite low. It’s generally not appropriate to make a constraint at exactly this priority. You want to be higher or lower.

## See Also

### Constants

static let required: UILayoutPriority

A required constraint.

static let defaultHigh: UILayoutPriority

The priority level with which a button resists compressing its content.

static let dragThatCanResizeScene: UILayoutPriority

The priority level for a drag that may end up resizing the window’s scene.

static let sceneSizeStayPut: UILayoutPriority

The priority level at which the window’s scene prefers to stay the same size.

static let dragThatCannotResizeScene: UILayoutPriority

The priority level for a drag that won’t resize the window’s scene.

static let defaultLow: UILayoutPriority

The priority level at which a button hugs its contents horizontally.

