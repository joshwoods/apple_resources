

- UIKit
- UIView
-  translatesAutoresizingMaskIntoConstraints 

Instance Property

# translatesAutoresizingMaskIntoConstraints

A Boolean value that determines whether the view’s autoresizing mask is translated into Auto Layout constraints.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var translatesAutoresizingMaskIntoConstraints: Bool { get set }
```

## Discussion

If this property’s value is true, the system creates a set of constraints that duplicate the behavior specified by the view’s autoresizing mask. This also lets you modify the view’s size and location using the view’s frame, bounds, or center properties, allowing you to create a static, frame-based layout within Auto Layout.

Note that the autoresizing mask constraints fully specify the view’s size and position; therefore, you cannot add additional constraints to modify this size or position without introducing conflicts. If you want to use Auto Layout to dynamically calculate the size and position of your view, you must set this property to false, and then provide a non ambiguous, nonconflicting set of constraints for the view.

By default, the property is set to true for any view you programmatically create. If you add views in Interface Builder, the system automatically sets this property to false.

## See Also

### Laying out subviews

func layoutSubviews()

Lays out subviews.

func setNeedsLayout()

Invalidates the current layout of the receiver and triggers a layout update during the next update cycle.

func layoutIfNeeded()

Lays out the subviews immediately, if layout updates are pending.

class var requiresConstraintBasedLayout: Bool

A Boolean value that indicates whether the receiver depends on the constraint-based layout system.

