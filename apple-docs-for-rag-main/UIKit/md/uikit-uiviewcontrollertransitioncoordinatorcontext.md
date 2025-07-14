

- UIKit
-  UIViewControllerTransitionCoordinatorContext 

Protocol

# UIViewControllerTransitionCoordinatorContext

A set of methods that provides information about an in-progress view controller transition.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIViewControllerTransitionCoordinatorContext : NSObjectProtocol
```

## Overview

Don’t adopt this protocol in your own classes. UIKit creates an object that adopts this protocol and makes it available to your code when you animate changes using a transition coordinator object.

A transition coordinator context provides most of the same information as an object that adopts the UIViewControllerContextTransitioning protocol. You use this contextual information to determine the animation parameters, such as the view in which the animations take place, whether the transition is interactive, or whether the transition was the result of an interface orientation change. You then apply that information to the animations you create.

Most animations take place in the view returned by the containerView method. And at the time your animation blocks are executed, the view hierarchy already contains the view of the *from* view controller. You can use your animation blocks to animate additional content in that same container view or you can animate content in an entirely different view.

## Topics

### Getting the views and view controllers

func viewController(forKey: UITransitionContextViewControllerKey) -> UIViewController?

Returns the view controllers involved in the transition.

**Required**

func view(forKey: UITransitionContextViewKey) -> UIView?

Returns the specified view involved in the transition.

**Required**

var containerView: UIView

Returns the view in which the transition takes place.

**Required**

### Getting the behavior attributes

var presentationStyle: UIModalPresentationStyle

The presentation style to use for the transition.

**Required**

var transitionDuration: TimeInterval

Returns the noninteractive duration of a transition.

**Required**

var completionCurve: UIView.AnimationCurve

Returns the completion curve associated with the transition.

**Required**

var completionVelocity: CGFloat

Returns the starting velocity to use for any final animations.

**Required**

var percentComplete: CGFloat

Returns the percentage of completion for an interactive transition when it moves to its noninteractive phase.

**Required**

### Getting the transition state

var initiallyInteractive: Bool

A Boolean value indicating whether the transition started as an interactive transition.

**Required**

var isInteractive: Bool

A Boolean value indicating whether the transition is currently interactive.

**Required**

var isAnimated: Bool

A Boolean value indicating whether the transition is explicitly animated.

**Required**

var isCancelled: Bool

A Boolean value indicating whether an interactive transition was canceled.

**Required**

var isInterruptible: Bool

A Boolean value indicating whether the transition animations can be interrupted.

**Required**

### Getting the rotation factor

var targetTransform: CGAffineTransform

Returns a transform indicating the amount of rotation being applied during the transition.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- UIViewControllerTransitionCoordinator

## See Also

### Transition coordinators

protocol UIViewControllerTransitionCoordinator

A set of methods that provides support for animations associated with a view controller transition.

