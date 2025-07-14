

- UIKit
- UICollisionBehavior
-  collisionDelegate 

Instance Property

# collisionDelegate

The delegate object that you want to respond to collisions for the collision behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var collisionDelegate: (any UICollisionBehaviorDelegate)? { get set }
```

## See Also

### Customizing the collision behavior

protocol UICollisionBehaviorDelegate

To respond to UIKit dynamic item collisions, configure a custom class to adopt the UICollisionBehaviorDelegate protocol. Then, in a collision behavior (an instance of the UICollisionBehavior class), set the delegate to be an instance of your custom class.

