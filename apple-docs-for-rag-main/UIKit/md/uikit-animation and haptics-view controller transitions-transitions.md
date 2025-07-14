

- UIKit
- Animation and haptics
-  View controller transitions 

API Collection

# View controller transitions

Define custom transitions from one view controller to another.

## Topics

### Essentials

Enhancing your app with fluid transitions

Use the fluid zoom transition to provide a continuously interactive and responsive experience in your app.

### Animation delegate

protocol UIViewControllerTransitioningDelegate

A set of methods that vend objects used to manage a fixed-length or interactive transition between view controllers.

### Non-interactive transitions

protocol UIViewControllerAnimatedTransitioning

A set of methods for implementing the animations for a custom view controller transition.

protocol UIViewControllerContextTransitioning

A set of methods that provide contextual information for transition animations between view controllers.

### Interactive transitions

class UIPercentDrivenInteractiveTransition

An object that drives an interactive animation between one view controller and another.

protocol UIViewControllerInteractiveTransitioning

A set of methods that enable an object (such as a navigation controller) to drive a view controller transition.

protocol UIViewImplicitlyAnimating

An interface for modifying an animation while it’s running.

### Transition coordinators

protocol UIViewControllerTransitionCoordinator

A set of methods that provides support for animations associated with a view controller transition.

protocol UIViewControllerTransitionCoordinatorContext

A set of methods that provides information about an in-progress view controller transition.

## See Also

### Content animations

Property-based animations

Create animations by changing the properties of a view.

Unifying your app’s animations

Create a consistent UI animation experience across SwiftUI, UIKit, and AppKit.

Optimizing ProMotion refresh rates for iPhone 13 Pro and iPad Pro

Provide custom animated content for ProMotion displays.

