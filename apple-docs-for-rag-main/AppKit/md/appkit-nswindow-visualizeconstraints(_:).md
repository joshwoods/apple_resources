

- AppKit
- NSWindow
-  visualizeConstraints(\_:) 

Instance Method

# visualizeConstraints(\_:)

Displays a visual representation of the supplied constraints in the window.

macOS 10.7+

``` source
@MainActor
func visualizeConstraints(_ constraints: [NSLayoutConstraint]?)
```

## Parameters 

`constraints`  

The constraints to visualize. All constraints must be held by views in the window.

## Discussion

The constraints to visualize are typically discovered by identifying a view whose layout is unexpected and then calling constraintsAffectingLayout(for:) on that view.

This method should only be used for debugging constraint-based layout. No application should ship with calls to this method as part of its operation.

