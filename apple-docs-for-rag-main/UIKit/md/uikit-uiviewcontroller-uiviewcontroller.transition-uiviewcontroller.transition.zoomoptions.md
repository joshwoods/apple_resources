

- UIKit
- UIViewController
- UIViewController.Transition
-  UIViewController.Transition.ZoomOptions 

Class

# UIViewController.Transition.ZoomOptions

Options for a zoom transition.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
class ZoomOptions
```

## Topics

### Setting options

var alignmentRectProvider: ((UIViewController.Transition.ZoomOptions.AlignmentRectContext) -> CGRect?)?

A closure that returns the alignment rectangle for the starting and ending views.

class AlignmentRectContext

An object that contains a zoom transition’s starting and ending views.

var dimmingColor: UIColor?

The dimming color.

var dimmingVisualEffect: UIBlurEffect?

The dimming visual effect.

### Accessing the animation state

var interactiveDismissShouldBegin: ((UIViewController.Transition.ZoomOptions.InteractionContext) -> Bool)?

A closure that determines whether an interactive dismissal can begin.

class InteractionContext

Data you can use to determine whether an interactive dismissal can begin.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Creating zoom transitions

static func zoom(options: UIViewController.Transition.ZoomOptions?, sourceViewProvider: (UIViewController.Transition.ZoomSourceViewProviderContext) -> UIView?) -> Self

Creates a zoom transition from the view that the source provider specifies.

class ZoomSourceViewProviderContext

A context object that contains references to the view controllers from a zoom transition.

