

- UIKit
- UIViewController
- UIViewController.Transition
-  UIViewController.Transition.ZoomSourceViewProviderContext 

Class

# UIViewController.Transition.ZoomSourceViewProviderContext

A context object that contains references to the view controllers from a zoom transition.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
class ZoomSourceViewProviderContext
```

## Topics

### Accessing the view controllers

var sourceViewController: UIViewController

The view controller that presents the zoomed view.

var zoomedViewController: UIViewController

The view controller for the presented view.

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

### Creating zoom transitions

static func zoom(options: UIViewController.Transition.ZoomOptions?, sourceViewProvider: (UIViewController.Transition.ZoomSourceViewProviderContext) -> UIView?) -> Self

Creates a zoom transition from the view that the source provider specifies.

class ZoomOptions

Options for a zoom transition.

