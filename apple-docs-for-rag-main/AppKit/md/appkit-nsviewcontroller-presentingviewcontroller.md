

- AppKit
- NSViewController
-  presentingViewController 

Instance Property

# presentingViewController

The view controller that presented the view controller or that presented its farthest ancestor view controller.

macOS 10.10+

``` source
@MainActor
unowned(unsafe) var presentingViewController: NSViewController? { get }
```

## Discussion

The *presenting view controller* is the one that is ultimately responsible for presenting the view controller whose presentingViewController property you are accessing.

## See Also

### Getting Related View Controllers

var parent: NSViewController?

The immediate ancestor view controller of the view controller.

var presentedViewControllers: [NSViewController]?

The view controllers, if any, that are currently presented by the view controller.

