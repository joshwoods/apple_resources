

- UIKit
-  UIDynamicAnimator 

Class

# UIDynamicAnimator

An object that provides physics-related capabilities and animations for its dynamic items, and provides the context for those animations.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
class UIDynamicAnimator
```

## Overview

A **dynamic item** is any iOS or custom object that conforms to the UIDynamicItem protocol. The UIView and UICollectionViewLayoutAttributes classes implement this protocol in iOS 7 and later. You can implement this protocol to use a dynamic animator with custom objects for such purposes as reacting to rotation or position changes computed by an animator.

To use dynamics, configure one or more dynamic behaviors—including providing each with a set of dynamic items—and then add those behaviors to a dynamic animator.

You specify dynamic behaviors using any of the iOS primitive dynamic behavior classes: UIAttachmentBehavior, UICollisionBehavior, UIDynamicItemBehavior, UIGravityBehavior, UIPushBehavior, and UISnapBehavior. Each of these provides configuration options and lets you associate one or more dynamic items to the behavior. To activate a behavior, add it to an animator.

A dynamic animator interacts with each of its dynamic items as follows:

1.  Before adding an item to a behavior, you specify the item’s starting position, rotation, and bounds (to do so, use properties of the item’s class, such as the center, transform, and bounds properties in the case of a UIView-based item)

2.  After you add the behavior to an animator, the animator takes over: it updates the item’s position and rotation as animation proceeds (see the UIDynamicItem protocol)

3.  You can programmatically update an item’s state in the midst of an animation, after which the animator takes back control of the item’s animation, relative to the state you specified (see the updateItem(usingCurrentState:) method)

You can define composite behaviors using the addChildBehavior(_:) method of the UIDynamicBehavior parent behavior class. The set of behaviors you add to an animator constitute a behavior hierarchy. Each behavior instance you associate with an animator can be present only once in the hierarchy.

To employ a dynamic animator, first identify the type of dynamic items you want to animate. This choice determines which initializer to call, and this in turn determines how the coordinate system gets set up. The three ways to initialize an animator, the dynamic items you can then use, and the resulting coordinate system, are as follows:

- To animate views, create an animator with the init(referenceView:) method. The coordinate system of the reference view serves as the coordinate system for the animator’s behaviors and items. Each dynamic item you associate with this sort of animator must be a UIView object and must descend from the reference view.

You can define a boundary, for items participating in a collision behavior, relative to the bounds of the reference view. See the setTranslatesReferenceBoundsIntoBoundary(with:) method.

- To animate collection views, create an animator with the init(collectionViewLayout:) method. The resulting animator employs a collection view layout (an object of the UICollectionViewLayout class) for its coordinate system. The dynamic items in this sort of animator must be UICollectionViewLayoutAttributes objects that are part of the layout.

You can define a boundary, for items participating in a collision behavior, relative to the bounds of the collection view layout. See the setTranslatesReferenceBoundsIntoBoundary(with:) method.

A collection view animator automatically calls the invalidateLayout() method as needed, and automatically pauses and resumes animation, as appropriate, when you change a collection view’s layout.

- To employ a dynamic animator with other objects that conform to the UIDynamicItem protocol, create an animator with the inherited init() method. The resulting animator employs an abstract coordinate system, not tied to the screen or to any view.

There is no reference boundary to refer to when defining a collision boundary for use with this sort of animator. However, you can still, in a collision behavior, specify custom boundaries as described in UICollisionBehavior.

All types of dynamic animators share the following characteristics:

- Each dynamic animator is independent of other dynamic animators you create

- You can associate a given dynamic item with multiple behaviors, provided those behaviors belong to the same animator

- An animator automatically pauses when all its items are at rest, and automatically resumes when a behavior parameter changes or a behavior or item is added or removed

You can implement a delegate to respond to changes in animator pause/resumption status, using the dynamicAnimatorDidPause(_:) and dynamicAnimatorWillResume(_:) methods of the UIDynamicAnimatorDelegate protocol.

## Topics

### Initializing and managing a dynamic animator

init(referenceView: UIView)

Initializes a dynamic animator with a specified view as its reference view.

convenience init(collectionViewLayout: UICollectionViewLayout)

Initializes a dynamic animator with a specified collection view layout.

func items(in: CGRect) -> [any UIDynamicItem]

Returns the dynamic items, from the animator’s behaviors, that intersect a specified rectangle.

func addBehavior(UIDynamicBehavior)

Adds a dynamic behavior to a dynamic animator.

func removeBehavior(UIDynamicBehavior)

Removes a specified dynamic behavior from a dynamic animator.

func removeAllBehaviors()

Removes all of the dynamic behaviors from a dynamic animator.

### Responding to animation changes

var delegate: (any UIDynamicAnimatorDelegate)?

The delegate for responding to pausing or resumption of animation.

protocol UIDynamicAnimatorDelegate

To respond to the pausing or resumption of UIKit dynamic animation, configure a custom class to adopt the UIDynamicAnimatorDelegate protocol. Then, in a dynamic animator (an instance of the UIDynamicAnimator class), set the delegate to be an instance of your custom class.

### Accessing a dynamic animator’s state

var elapsedTime: TimeInterval

Returns the time interval since the dynamic animator started running.

var isRunning: Bool

Returns true if the dynamic animator is running.

var behaviors: [UIDynamicBehavior]

The dynamic behaviors managed by a dynamic animator.

var referenceView: UIView?

The view that a dynamic animator was initialized with.

func updateItem(usingCurrentState: any UIDynamicItem)

Asks a dynamic animator to read the current state of a dynamic item, replacing the animator’s internal representation of the item’s state.

### Working with collection views

func layoutAttributesForCell(at: IndexPath) -> UICollectionViewLayoutAttributes?

A convenience method for returning the layout attributes for a collection view cell.

func layoutAttributesForDecorationView(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

A convenience method for returning the layout attributes for a collection view decoration view.

func layoutAttributesForSupplementaryView(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

A convenience method for returning the layout attributes for a collection view supplementary view.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

