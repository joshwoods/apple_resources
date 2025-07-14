

- AppKit
- NSView
-  requiresConstraintBasedLayout 

Type Property

# requiresConstraintBasedLayout

Returns a Boolean value indicating whether the view depends on the constraint-based layout system.

macOS 10.7+

``` source
@MainActor
class var requiresConstraintBasedLayout: Bool { get }
```

## Return Value

true if the view must be in a window using constraint-based layout to function properly, false otherwise.

## Discussion

Custom views should override this to return true if they can not layout correctly using autoresizing.

## See Also

### Opting In to Auto Layout

var translatesAutoresizingMaskIntoConstraints: Bool

A Boolean value indicating whether the view’s autoresizing mask is translated into constraints for the constraint-based layout system.

