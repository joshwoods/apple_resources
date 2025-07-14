

- AppKit
- NSLayoutConstraint
-  isActive 

Instance Property

# isActive

The active state of the constraint.

macOS 10.10+

``` source
var isActive: Bool { get set }
```

## Discussion

You can activate or deactivate a constraint by changing this property. Note that only active constraints affect the calculated layout. If you try to activate a constraint whose items have no common ancestor, an exception is thrown. For newly created constraints, the isActive property is false by default.

Activating or deactivating the constraint calls addConstraint(_:) and removeConstraint(_:) on the view that is the closest common ancestor of the items managed by this constraint. Use this property instead of calling addConstraint(_:) or removeConstraint(_:) directly.

## See Also

### Activating and deactivating constraints

class func activate([NSLayoutConstraint])

Activates each constraint in the specified array.

class func deactivate([NSLayoutConstraint])

Deactivates each constraint in the specified array.

