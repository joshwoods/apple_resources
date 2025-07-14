

- UIKit
- UIView
-  layoutIfNeeded() 

Instance Method

# layoutIfNeeded()

Lays out the subviews immediately, if layout updates are pending.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func layoutIfNeeded()
```

## Discussion

Use this method to force the view to update its layout immediately. When using Auto Layout, the layout engine updates the position of views as needed to satisfy changes in constraints. Using the view that receives the message as the root view, this method lays out the view subtree starting at the root. If no layout updates are pending, this method exits without modifying the layout or calling any layout-related callbacks.

## See Also

### Laying out subviews

func layoutSubviews()

Lays out subviews.

func setNeedsLayout()

Invalidates the current layout of the receiver and triggers a layout update during the next update cycle.

class var requiresConstraintBasedLayout: Bool

A Boolean value that indicates whether the receiver depends on the constraint-based layout system.

var translatesAutoresizingMaskIntoConstraints: Bool

A Boolean value that determines whether the view’s autoresizing mask is translated into Auto Layout constraints.

