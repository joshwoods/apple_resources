

- UIKit
- UIViewController
- UIViewController.Transition
- UIViewController.Transition.ZoomOptions
-  dimmingVisualEffect 

Instance Property

# dimmingVisualEffect

The dimming visual effect.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
var dimmingVisualEffect: UIBlurEffect? { get set }
```

## See Also

### Setting options

var alignmentRectProvider: ((UIViewController.Transition.ZoomOptions.AlignmentRectContext) -> CGRect?)?

A closure that returns the alignment rectangle for the starting and ending views.

class AlignmentRectContext

An object that contains a zoom transition’s starting and ending views.

var dimmingColor: UIColor?

The dimming color.

