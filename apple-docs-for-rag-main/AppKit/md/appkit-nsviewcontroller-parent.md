

- AppKit
- NSViewController
-  parent 

Instance Property

# parent

The immediate ancestor view controller of the view controller.

macOS 10.10+

``` source
@MainActor
var parent: NSViewController? { get }
```

## Discussion

The value of this property is `nil` if the view controller has no parent view controller, such as if the view controller is a window’s content view controller.

## See Also

### Getting Related View Controllers

var presentedViewControllers: [NSViewController]?

The view controllers, if any, that are currently presented by the view controller.

var presentingViewController: NSViewController?

The view controller that presented the view controller or that presented its farthest ancestor view controller.

