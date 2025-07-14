

- AppKit
- NSView
-  constraints 

Instance Property

# constraints

Returns the constraints held by the view.

macOS 10.7+

``` source
@MainActor
var constraints: [NSLayoutConstraint] { get }
```

## Return Value

The constraints held by the view.

## See Also

### Managing the View’s Constraints

func addConstraint(NSLayoutConstraint)

Adds a constraint on the layout of the receiving view or its subviews.

func addConstraints([NSLayoutConstraint])

Adds multiple constraints on the layout of the receiving view or its subviews.

func removeConstraint(NSLayoutConstraint)

Removes the specified constraint from the view.

func removeConstraints([NSLayoutConstraint])

Removes the specified constraints from the view.

