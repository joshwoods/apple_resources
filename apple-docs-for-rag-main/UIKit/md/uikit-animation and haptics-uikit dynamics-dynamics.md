

- UIKit
- Animation and haptics
-  UIKit Dynamics 

API Collection

# UIKit Dynamics

Apply physics-based animations to your views.

## Topics

### Dynamic animators

class UIDynamicAnimator

An object that provides physics-related capabilities and animations for its dynamic items, and provides the context for those animations.

### Dynamic Items

protocol UIDynamicItem

A set of methods that can make a custom object eligible to participate in UIKit Dynamics.

class UIDynamicItemBehavior

A base dynamic animation configuration for one or more dynamic items.

class UIDynamicItemGroup

A dynamic item that comprises multiple other dynamic items.

### Behaviors

class UIDynamicBehavior

An object that confers a behavioral configuration on one or more dynamic items, for their participation in 2D animation.

class UIAttachmentBehavior

A relationship between two dynamic items, or between a dynamic item and an anchor point.

class UICollisionBehavior

An object that confers to a specified array of dynamic items the ability to engage in collisions with each other and with the behavior’s specified boundaries.

class UIFieldBehavior

An object that applies field-based physics to dynamic items.

class UIGravityBehavior

An object that applies a gravity-like force to all of its associated dynamic items.

class UIPushBehavior

A behavior that applies a continuous or instantaneous force to one or more dynamic items, causing those items to change position accordingly.

class UISnapBehavior

A spring-like behavior whose initial motion is damped over time so that the object settles at a specific point.

### Animation regions

class UIRegion

A shape for use in UIKit Dynamics.

