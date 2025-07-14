

- UIKit
- UILayoutGuide
-  hasAmbiguousLayout 

Instance Property

# hasAmbiguousLayout

A Boolean value indicating whether the constraints impacting the layout guide specify its location ambiguously.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var hasAmbiguousLayout: Bool { get }
```

## See Also

### Debugging the layout guide

func constraintsAffectingLayout(for: NSLayoutConstraint.Axis) -> [NSLayoutConstraint]

The constraints that impact the layout of the guide.

