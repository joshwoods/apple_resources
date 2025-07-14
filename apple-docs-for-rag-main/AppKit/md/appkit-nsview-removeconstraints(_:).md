

- AppKit
- NSView
-  removeConstraints(\_:) 

Instance Method

# removeConstraints(\_:)

Removes the specified constraints from the view.

macOS 10.7+

``` source
@MainActor
func removeConstraints(_ constraints: [NSLayoutConstraint])
```

## Parameters 

`constraints`  

The constraints to remove.

## See Also

### Managing the View’s Constraints

var constraints: [NSLayoutConstraint]

Returns the constraints held by the view.

func addConstraint(NSLayoutConstraint)

Adds a constraint on the layout of the receiving view or its subviews.

func addConstraints([NSLayoutConstraint])

Adds multiple constraints on the layout of the receiving view or its subviews.

func removeConstraint(NSLayoutConstraint)

Removes the specified constraint from the view.

