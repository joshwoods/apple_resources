

- UIKit
- UILayoutGuide
-  constraintsAffectingLayout(for:) 

Instance Method

# constraintsAffectingLayout(for:)

The constraints that impact the layout of the guide.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
func constraintsAffectingLayout(for axis: NSLayoutConstraint.Axis) -> [NSLayoutConstraint]
```

## See Also

### Debugging the layout guide

var hasAmbiguousLayout: Bool

A Boolean value indicating whether the constraints impacting the layout guide specify its location ambiguously.

