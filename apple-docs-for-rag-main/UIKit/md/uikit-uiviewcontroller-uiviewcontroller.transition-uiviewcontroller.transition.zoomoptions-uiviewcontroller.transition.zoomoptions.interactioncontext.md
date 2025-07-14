

- UIKit
- UIViewController
- UIViewController.Transition
- UIViewController.Transition.ZoomOptions
-  UIViewController.Transition.ZoomOptions.InteractionContext 

Class

# UIViewController.Transition.ZoomOptions.InteractionContext

Data you can use to determine whether an interactive dismissal can begin.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
class InteractionContext
```

## Topics

### Accessing the context

var location: CGPoint

The touch’s location.

var velocity: CGVector

The touch’s velocity.

var willBegin: Bool

A Boolean value that indicates whether the transition is beginning.

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

## See Also

### Accessing the animation state

var interactiveDismissShouldBegin: ((UIViewController.Transition.ZoomOptions.InteractionContext) -> Bool)?

A closure that determines whether an interactive dismissal can begin.

