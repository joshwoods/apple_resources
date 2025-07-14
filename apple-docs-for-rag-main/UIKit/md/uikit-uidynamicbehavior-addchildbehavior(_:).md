

- UIKit
- UIDynamicBehavior
-  addChildBehavior(\_:) 

Instance Method

# addChildBehavior(\_:)

Adds a dynamic behavior, as a child, to a custom dynamic behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func addChildBehavior(_ behavior: UIDynamicBehavior)
```

## Parameters 

`behavior`  

The dynamic behavior you want to add as a child.

The parent behavior ignores your use of this method if you:

- Provide a `nil` value

- Provide a behavior instance that you’ve already added to the behavior

## Discussion

Call this method only on custom subclasses of the UIDynamicBehavior class.

## See Also

### Configuring a dynamic behavior

var action: (() -> Void)?

The block you want to execute during dynamic animation.

var childBehaviors: [UIDynamicBehavior]

Returns the array of dynamic behaviors that are children of a custom dynamic behavior.

func removeChildBehavior(UIDynamicBehavior)

Removes a child dynamic behavior from a custom dynamic behavior.

