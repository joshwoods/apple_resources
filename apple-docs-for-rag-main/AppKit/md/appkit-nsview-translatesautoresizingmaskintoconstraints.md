

- AppKit
- NSView
-  translatesAutoresizingMaskIntoConstraints 

Instance Property

# translatesAutoresizingMaskIntoConstraints

A Boolean value indicating whether the view’s autoresizing mask is translated into constraints for the constraint-based layout system.

macOS 10.7+

``` source
@MainActor
var translatesAutoresizingMaskIntoConstraints: Bool { get set }
```

## Discussion

When this property is set to true, the view’s superview looks at the view’s autoresizing mask, produces constraints that implement it, and adds those constraints to itself (the superview). If your view has flexible constraints that require dynamic adjustment, set this property to false and apply the constraints yourself.

## See Also

### Opting In to Auto Layout

class var requiresConstraintBasedLayout: Bool

Returns a Boolean value indicating whether the view depends on the constraint-based layout system.

