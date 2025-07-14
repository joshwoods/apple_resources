

- UIKit
- UIViewController
- UIViewController.Transition
- UIViewController.Transition.ZoomOptions
-  UIViewController.Transition.ZoomOptions.AlignmentRectContext 

Class

# UIViewController.Transition.ZoomOptions.AlignmentRectContext

An object that contains a zoom transition’s starting and ending views.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
class AlignmentRectContext
```

## Topics

### Accessing views

var sourceView: UIView

The zoomed-out view, for example a thumbnail image.

var zoomedViewController: UIViewController

The zoomed in view.

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

### Setting options

var alignmentRectProvider: ((UIViewController.Transition.ZoomOptions.AlignmentRectContext) -> CGRect?)?

A closure that returns the alignment rectangle for the starting and ending views.

var dimmingColor: UIColor?

The dimming color.

var dimmingVisualEffect: UIBlurEffect?

The dimming visual effect.

