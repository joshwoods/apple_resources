

- AppKit
- NSLayoutAnchor
-  constraintsAffectingLayout 

Instance Property

# constraintsAffectingLayout

The constraints that impact the layout of the anchor.

macOS 10.12+

``` source
var constraintsAffectingLayout: [NSLayoutConstraint] { get }
```

## See Also

### Debugging the anchor

var hasAmbiguousLayout: Bool

A Boolean value indicating whether the constraints impacting the anchor specify its location ambiguously.

var name: String

The name assigned to the anchor for debugging purposes.

var item: AnyObject?

The layout item used to calculate the anchor’s position.

