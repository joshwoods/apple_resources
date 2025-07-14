

- UIKit
- UIView
-  constraintsAffectingLayout(for:) 

Instance Method

# constraintsAffectingLayout(for:)

Returns the constraints impacting the layout of the view for a given axis.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func constraintsAffectingLayout(for axis: NSLayoutConstraint.Axis) -> [NSLayoutConstraint]
```

## Parameters 

`axis`  

The axis for which the constraints should be found.

## Return Value

The constraints impacting the layout of the view for the specified axis.

## Discussion

The returned set of constraints may not all include the view explicitly. Constraints that impact the location of the view implicitly may also be included. While this provides a good starting point for debugging, there is no guarantee that the returned set of constraints will include all of the constraints that have an impact on the view’s layout in the given orientation.

This method should only be used for debugging constraint-based layout. No application should ship with calls to this method as part of its operation.

## See Also

### Debugging Auto Layout

var hasAmbiguousLayout: Bool

A Boolean value that determines whether the constraints impacting the layout of the view incompletely specify the location of the view.

func exerciseAmbiguityInLayout()

Randomly changes the frame of a view with an ambiguous layout between the different valid values.

