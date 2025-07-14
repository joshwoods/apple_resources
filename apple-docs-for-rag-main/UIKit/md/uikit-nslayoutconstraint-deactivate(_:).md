

- UIKit
- NSLayoutConstraint
-  deactivate(\_:) 

Type Method

# deactivate(\_:)

Deactivates each constraint in the specified array.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class func deactivate(_ constraints: [NSLayoutConstraint])
```

## Parameters 

`constraints`  

An array of constraints to deactivate.

## Discussion

This is a convenience method that provides an easy way to deactivate a set of constraints with one call. The effect of this method is the same as setting the isActive property of each constraint to false. Typically, using this method is more efficient than deactivating each constraint individually.

## See Also

### Activating and deactivating constraints

var isActive: Bool

The active state of the constraint.

class func activate([NSLayoutConstraint])

Activates each constraint in the specified array.

