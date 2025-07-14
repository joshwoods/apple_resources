

- AppKit
- NSLayoutAnchor
-  hasAmbiguousLayout 

Instance Property

# hasAmbiguousLayout

A Boolean value indicating whether the constraints impacting the anchor specify its location ambiguously.

macOS 10.12+

``` source
var hasAmbiguousLayout: Bool { get }
```

## See Also

### Debugging the anchor

var constraintsAffectingLayout: [NSLayoutConstraint]

The constraints that impact the layout of the anchor.

var name: String

The name assigned to the anchor for debugging purposes.

var item: AnyObject?

The layout item used to calculate the anchor’s position.

