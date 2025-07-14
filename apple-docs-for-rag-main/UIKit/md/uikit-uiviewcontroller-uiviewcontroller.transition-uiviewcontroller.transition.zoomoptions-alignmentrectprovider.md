

- UIKit
- UIViewController
- UIViewController.Transition
- UIViewController.Transition.ZoomOptions
-  alignmentRectProvider 

Instance Property

# alignmentRectProvider

A closure that returns the alignment rectangle for the starting and ending views.

iOS 18.0+iPadOS 18.0+Mac CatalysttvOSvisionOS

``` source
var alignmentRectProvider: ((UIViewController.Transition.ZoomOptions.AlignmentRectContext) -> CGRect?)? { get set }
```

## See Also

### Setting options

class AlignmentRectContext

An object that contains a zoom transition’s starting and ending views.

var dimmingColor: UIColor?

The dimming color.

var dimmingVisualEffect: UIBlurEffect?

The dimming visual effect.

