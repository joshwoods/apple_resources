

- UIKit
- UIView
-  removeConstraints(\_:) 

Instance Method

# removeConstraints(\_:)

Removes the specified constraints from the view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func removeConstraints(_ constraints: [NSLayoutConstraint])
```

## Parameters 

`constraints`  

The constraints to remove.

## Discussion

When developing for iOS 8.0 or later, use the NSLayoutConstraint class’s deactivate(_:) method instead of calling the removeConstraints(_:) method directly. The deactivate(_:) method automatically removes the constraints from the correct views.

## See Also

### Managing the view’s constraints

var constraints: [NSLayoutConstraint]

The constraints held by the view.

func addConstraint(NSLayoutConstraint)

Adds a constraint on the layout of the receiving view or its subviews.

func addConstraints([NSLayoutConstraint])

Adds multiple constraints on the layout of the receiving view or its subviews.

func removeConstraint(NSLayoutConstraint)

Removes the specified constraint from the view.

