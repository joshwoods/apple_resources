

- AppKit
- NSPageController
-  delegate 

Instance Property

# delegate

The page controller’s delegate object.

macOS 10.8+

``` source
@IBOutlet @MainActor
weak var delegate: (any NSPageControllerDelegate)? { get set }
```

## Discussion

The delegate must conform to the NSPageControllerDelegate protocol.

## See Also

### Customizing the Paged Interface Behavior

protocol NSPageControllerDelegate

The `NSPageControllerDelegate` protocol allows you to customize the behavior of instances of the NSPageController class.

