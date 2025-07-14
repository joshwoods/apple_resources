

- AppKit
- NSLayoutAnchor
-  name 

Instance Property

# name

The name assigned to the anchor for debugging purposes.

macOS 10.12+

``` source
var name: String { get }
```

## See Also

### Debugging the anchor

var constraintsAffectingLayout: [NSLayoutConstraint]

The constraints that impact the layout of the anchor.

var hasAmbiguousLayout: Bool

A Boolean value indicating whether the constraints impacting the anchor specify its location ambiguously.

var item: AnyObject?

The layout item used to calculate the anchor’s position.

