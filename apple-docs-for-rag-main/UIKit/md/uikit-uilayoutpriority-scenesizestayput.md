

- UIKit
- UILayoutPriority
-  sceneSizeStayPut 

Type Property

# sceneSizeStayPut

The priority level at which the window’s scene prefers to stay the same size.

iOSiPadOSMac Catalyst 13.0+tvOSvisionOS

``` source
static let sceneSizeStayPut: UILayoutPriority
```

## Discussion

Specify constraint priorities that are either higher or lower than this value, rather than equal to it.

## See Also

### Constants

static let required: UILayoutPriority

A required constraint.

static let defaultHigh: UILayoutPriority

The priority level with which a button resists compressing its content.

static let dragThatCanResizeScene: UILayoutPriority

The priority level for a drag that may end up resizing the window’s scene.

static let dragThatCannotResizeScene: UILayoutPriority

The priority level for a drag that won’t resize the window’s scene.

static let defaultLow: UILayoutPriority

The priority level at which a button hugs its contents horizontally.

static let fittingSizeLevel: UILayoutPriority

The priority level with which the view wants to conform to the target size in that computation.

