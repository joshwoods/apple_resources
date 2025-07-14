

- AppKit
- NSView
-  addConstraints(\_:) 

Instance Method

# addConstraints(\_:)

Adds multiple constraints on the layout of the receiving view or its subviews.

macOS 10.7+

``` source
@MainActor
func addConstraints(_ constraints: [NSLayoutConstraint])
```

## Parameters 

`constraints`  

An array of constraints to be added to the view. All constraints may only reference the view itself or its subviews.

## Discussion

All constraints must involve only views that are within scope of the receiving view. Specifically, any views involved must be either the receiving view itself, or a subview of the receiving view. Constraints that are added to a view are said to be held by that view. The coordinate system used when evaluating each constraint is the coordinate system of the view that holds the constraint.

## See Also

### Managing the View’s Constraints

var constraints: [NSLayoutConstraint]

Returns the constraints held by the view.

func addConstraint(NSLayoutConstraint)

Adds a constraint on the layout of the receiving view or its subviews.

func removeConstraint(NSLayoutConstraint)

Removes the specified constraint from the view.

func removeConstraints([NSLayoutConstraint])

Removes the specified constraints from the view.

