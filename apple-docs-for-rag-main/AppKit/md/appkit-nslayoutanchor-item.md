

- AppKit
- NSLayoutAnchor
-  item 

Instance Property

# item

The layout item used to calculate the anchor’s position.

macOS 10.12+

``` source
weak var item: AnyObject? { get }
```

## See Also

### Debugging the anchor

var constraintsAffectingLayout: [NSLayoutConstraint]

The constraints that impact the layout of the anchor.

var hasAmbiguousLayout: Bool

A Boolean value indicating whether the constraints impacting the anchor specify its location ambiguously.

var name: String

The name assigned to the anchor for debugging purposes.

