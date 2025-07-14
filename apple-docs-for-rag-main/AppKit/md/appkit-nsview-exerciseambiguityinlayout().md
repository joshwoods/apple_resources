

- AppKit
- NSView
-  exerciseAmbiguityInLayout() 

Instance Method

# exerciseAmbiguityInLayout()

Randomly changes the frame of a view with an ambiguous layout between the different valid values.

macOS 10.7+

``` source
@MainActor
func exerciseAmbiguityInLayout()
```

## Discussion

This method randomly changes the frame of a view with an ambiguous layout between its different valid values, causing the view to move in the interface. This makes it easy to visually identify what the valid frames are and may enable the developer to discern what constraints need to be added to the layout to fully specify a location for the view.

This method should only be used for debugging constraint-based layout. No application should ship with calls to this method as part of its operation.

## See Also

### Debugging Auto Layout

func constraintsAffectingLayout(for: NSLayoutConstraint.Orientation) -> [NSLayoutConstraint]

Returns the constraints impacting the layout of the view for a given orientation.

var hasAmbiguousLayout: Bool

A Boolean value indicating whether the constraints impacting the layout of the view incompletely specify the location of the view.

