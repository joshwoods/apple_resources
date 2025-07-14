

- AppKit
- NSLayoutConstraint
-  activate(\_:) 

Type Method

# activate(\_:)

Activates each constraint in the specified array.

macOS 10.10+

``` source
class func activate(_ constraints: [NSLayoutConstraint])
```

## Parameters 

`constraints`  

An array of constraints to activate.

## Discussion

This convenience method provides an easy way to activate a set of constraints with one call. The effect of this method is the same as setting the isActive property of each constraint to true. Typically, using this method is more efficient than activating each constraint individually.

## See Also

### Activating and deactivating constraints

var isActive: Bool

The active state of the constraint.

class func deactivate([NSLayoutConstraint])

Deactivates each constraint in the specified array.

