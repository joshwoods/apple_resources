

- UIKit
- UIViewController
- UIViewController.Transition
- UIViewController.Transition.ZoomOptions
-  interactiveDismissShouldBegin 

Instance Property

# interactiveDismissShouldBegin

A closure that determines whether an interactive dismissal can begin.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
var interactiveDismissShouldBegin: ((UIViewController.Transition.ZoomOptions.InteractionContext) -> Bool)? { get set }
```

## See Also

### Accessing the animation state

class InteractionContext

Data you can use to determine whether an interactive dismissal can begin.

