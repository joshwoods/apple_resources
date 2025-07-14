

- UIKit
- UIDynamicBehavior
-  childBehaviors 

Instance Property

# childBehaviors

Returns the array of dynamic behaviors that are children of a custom dynamic behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var childBehaviors: [UIDynamicBehavior] { get }
```

## Discussion

Only custom subclasses of the class can have child behaviors.

## See Also

### Configuring a dynamic behavior

var action: (() -> Void)?

The block you want to execute during dynamic animation.

func addChildBehavior(UIDynamicBehavior)

Adds a dynamic behavior, as a child, to a custom dynamic behavior.

func removeChildBehavior(UIDynamicBehavior)

Removes a child dynamic behavior from a custom dynamic behavior.

