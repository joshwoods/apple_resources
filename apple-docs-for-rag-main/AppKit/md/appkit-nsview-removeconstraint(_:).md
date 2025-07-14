

- AppKit
- NSView
-  removeConstraint(\_:) 

Instance Method

# removeConstraint(\_:)

Removes the specified constraint from the view.

macOS 10.7+

``` source
@MainActor
func removeConstraint(_ constraint: NSLayoutConstraint)
```

## Parameters 

`constraint`  

The constraint to remove. Removing a constraint not held by the view has no effect.

## See Also

### Managing the View’s Constraints

var constraints: [NSLayoutConstraint]

Returns the constraints held by the view.

func addConstraint(NSLayoutConstraint)

Adds a constraint on the layout of the receiving view or its subviews.

func addConstraints([NSLayoutConstraint])

Adds multiple constraints on the layout of the receiving view or its subviews.

func removeConstraints([NSLayoutConstraint])

Removes the specified constraints from the view.

