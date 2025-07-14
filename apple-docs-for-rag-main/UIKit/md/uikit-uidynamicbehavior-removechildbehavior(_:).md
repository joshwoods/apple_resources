

- UIKit
- UIDynamicBehavior
-  removeChildBehavior(\_:) 

Instance Method

# removeChildBehavior(\_:)

Removes a child dynamic behavior from a custom dynamic behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func removeChildBehavior(_ behavior: UIDynamicBehavior)
```

## Parameters 

`behavior`  

The child dynamic behavior you want to remove.

The parent behavior ignores your use of this method if you:

- Provide a `nil` value

- Provide a behavior instance that is not a child of the parent behavior

## Discussion

This method applies only to custom subclasses of the UIDynamicBehavior class. UIKit concrete dynamic behaviors (such as an instance of UICollisionBehavior) cannot have child behaviors.

## See Also

### Configuring a dynamic behavior

var action: (() -> Void)?

The block you want to execute during dynamic animation.

func addChildBehavior(UIDynamicBehavior)

Adds a dynamic behavior, as a child, to a custom dynamic behavior.

var childBehaviors: [UIDynamicBehavior]

Returns the array of dynamic behaviors that are children of a custom dynamic behavior.

