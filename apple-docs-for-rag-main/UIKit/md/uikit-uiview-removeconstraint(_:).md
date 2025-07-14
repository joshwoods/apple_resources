

- UIKit
- UIView
-  removeConstraint(\_:) 

Instance Method

# removeConstraint(\_:)

Removes the specified constraint from the view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func removeConstraint(_ constraint: NSLayoutConstraint)
```

## Parameters 

`constraint`  

The constraint to remove. Removing a constraint not held by the view has no effect.

## Discussion

When developing for iOS 8.0 or later, set the constraint’s isActive property to false instead of calling the removeConstraint(_:) method directly. The isActive property automatically adds and removes the constraint from the correct view.

## See Also

### Managing the view’s constraints

var constraints: [NSLayoutConstraint]

The constraints held by the view.

func addConstraint(NSLayoutConstraint)

Adds a constraint on the layout of the receiving view or its subviews.

func addConstraints([NSLayoutConstraint])

Adds multiple constraints on the layout of the receiving view or its subviews.

func removeConstraints([NSLayoutConstraint])

Removes the specified constraints from the view.

