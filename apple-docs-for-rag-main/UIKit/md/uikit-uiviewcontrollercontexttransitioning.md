

- UIKit
-  UIViewControllerContextTransitioning 

Protocol

# UIViewControllerContextTransitioning

A set of methods that provide contextual information for transition animations between view controllers.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIViewControllerContextTransitioning : NSObjectProtocol
```

## Overview

Don’t adopt this protocol in your own classes, nor should you directly create objects that adopt this protocol. During a transition, the animator objects involved in that transition receive a fully configured context object from UIKit. Custom animator objects — objects that adopt the UIViewControllerAnimatedTransitioning or UIViewControllerInteractiveTransitioning protocol — should simply retrieve the information they need from the provided object.

A context object encapsulates information about the views and view controllers involved in the transition. It also contains details about the how to execute the transition. For interactive transitions, the interactive animator object uses the methods of this protocol to report the animation’s progress. When the animation starts, the interactive animator object must save a pointer to the context object. Based on user interactions, the animator object then calls the updateInteractiveTransition(_:), finishInteractiveTransition(), or cancelInteractiveTransition() methods to report the progress toward completing the animation. Those methods send that information to UIKit so that it can drive the timing of the animations.

Important

When defining custom animator objects, always check the value returned by the isAnimated method to determine whether you should create animations at all. And when you do create transition animations, always call the completeTransition(_:) method from an appropriate completion block to let UIKit know when all of your animations have finished.

## Topics

### Accessing the transition objects

var containerView: UIView

The view that acts as the superview for the views involved in the transition.

**Required**

func viewController(forKey: UITransitionContextViewControllerKey) -> UIViewController?

Returns a view controller involved in the transition.

**Required**

func view(forKey: UITransitionContextViewKey) -> UIView?

Returns the specified view involved in the transition.

**Required**

### Getting the transition frame rectangles

func initialFrame(for: UIViewController) -> CGRect

Returns the starting frame rectangle for the specified view controller’s view.

**Required**

func finalFrame(for: UIViewController) -> CGRect

Returns the ending frame rectangle for the specified view controller’s view.

**Required**

### Getting the transition behaviors

var isAnimated: Bool

A Boolean value indicating whether the transition should be animated.

**Required**

var isInteractive: Bool

A Boolean value indicating whether the transition is currently interactive.

**Required**

var presentationStyle: UIModalPresentationStyle

Returns the presentation style for the view controller transition.

**Required**

### Reporting the transition progress

func completeTransition(Bool)

Notifies the system that the transition animation is done.

**Required**

func updateInteractiveTransition(CGFloat)

Updates the completion percentage of the transition.

**Required**

func pauseInteractiveTransition()

Tells the system to pause the animations.

**Required**

func finishInteractiveTransition()

Notifies the system that user interactions signaled the completion of the transition.

**Required**

func cancelInteractiveTransition()

Notifies the system that user interactions canceled the transition.

**Required**

var transitionWasCancelled: Bool

Returns a Boolean value indicating whether the transition was canceled.

**Required**

### Getting the rotation factor

var targetTransform: CGAffineTransform

Returns a transform indicating the amount of rotation being applied during the transition.

**Required**

### Constants

struct UITransitionContextViewControllerKey

The keys you use to identify the view controllers involved in a transition.

struct UITransitionContextViewKey

The keys you use to identify the views involved in a transition.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Non-interactive transitions

protocol UIViewControllerAnimatedTransitioning

A set of methods for implementing the animations for a custom view controller transition.

