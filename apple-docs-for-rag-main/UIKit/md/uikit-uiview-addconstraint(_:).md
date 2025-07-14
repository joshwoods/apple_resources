

- UIKit
- UIView
-  addConstraint(\_:) 

Instance Method

# addConstraint(\_:)

Adds a constraint on the layout of the receiving view or its subviews.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func addConstraint(_ constraint: NSLayoutConstraint)
```

## Parameters 

`constraint`  

The constraint to be added to the view. The constraint may only reference the view itself or its subviews.

## Discussion

The constraint must involve only views that are within scope of the receiving view. Specifically, any views involved must be either the receiving view itself, or a subview of the receiving view. Constraints that are added to a view are said to be held by that view. The coordinate system used when evaluating the constraint is the coordinate system of the view that holds the constraint.

When developing for iOS 8.0 or later, set the constraint’s isActive property to true instead of calling the addConstraint(_:) method directly. The isActive property automatically adds and removes the constraint from the correct view.

## See Also

### Managing the view’s constraints

var constraints: [NSLayoutConstraint]

The constraints held by the view.

func addConstraints([NSLayoutConstraint])

Adds multiple constraints on the layout of the receiving view or its subviews.

func removeConstraint(NSLayoutConstraint)

Removes the specified constraint from the view.

func removeConstraints([NSLayoutConstraint])

Removes the specified constraints from the view.

