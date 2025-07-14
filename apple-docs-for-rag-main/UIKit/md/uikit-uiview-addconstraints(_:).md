

- UIKit
- UIView
-  addConstraints(\_:) 

Instance Method

# addConstraints(\_:)

Adds multiple constraints on the layout of the receiving view or its subviews.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func addConstraints(_ constraints: [NSLayoutConstraint])
```

## Parameters 

`constraints`  

An array of constraints to be added to the view. All constraints may only reference the view itself or its subviews.

## Discussion

All constraints must involve only views that are within scope of the receiving view. Specifically, any views involved must be either the receiving view itself, or a subview of the receiving view. Constraints that are added to a view are said to be held by that view. The coordinate system used when evaluating each constraint is the coordinate system of the view that holds the constraint.

When developing for iOS 8.0 or later, use the NSLayoutConstraint class’s activate(_:) method instead of calling the addConstraints(_:) method directly. The activate(_:) method automatically adds the constraints to the correct views.

## See Also

### Managing the view’s constraints

var constraints: [NSLayoutConstraint]

The constraints held by the view.

func addConstraint(NSLayoutConstraint)

Adds a constraint on the layout of the receiving view or its subviews.

func removeConstraint(NSLayoutConstraint)

Removes the specified constraint from the view.

func removeConstraints([NSLayoutConstraint])

Removes the specified constraints from the view.

