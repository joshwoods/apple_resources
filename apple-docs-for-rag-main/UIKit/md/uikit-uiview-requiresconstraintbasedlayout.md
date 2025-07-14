

- UIKit
- UIView
-  requiresConstraintBasedLayout 

Type Property

# requiresConstraintBasedLayout

A Boolean value that indicates whether the receiver depends on the constraint-based layout system.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class var requiresConstraintBasedLayout: Bool { get }
```

## Return Value

true if the view must be in a window using constraint-based layout to function properly, false otherwise.

## Discussion

Custom views should override this to return true if they cannot layout correctly using autoresizing.

## See Also

### Laying out subviews

func layoutSubviews()

Lays out subviews.

func setNeedsLayout()

Invalidates the current layout of the receiver and triggers a layout update during the next update cycle.

func layoutIfNeeded()

Lays out the subviews immediately, if layout updates are pending.

var translatesAutoresizingMaskIntoConstraints: Bool

A Boolean value that determines whether the view’s autoresizing mask is translated into Auto Layout constraints.

