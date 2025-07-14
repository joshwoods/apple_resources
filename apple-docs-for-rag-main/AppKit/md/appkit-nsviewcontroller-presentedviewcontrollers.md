

- AppKit
- NSViewController
-  presentedViewControllers 

Instance Property

# presentedViewControllers

The view controllers, if any, that are currently presented by the view controller.

macOS 10.10+

``` source
@MainActor
var presentedViewControllers: [NSViewController]? { get }
```

## Discussion

There is a one-to-many relationship between the view controller whose presentedViewControllers property you are accessing, and the view controllers it is currently presenting.

## See Also

### Getting Related View Controllers

var parent: NSViewController?

The immediate ancestor view controller of the view controller.

var presentingViewController: NSViewController?

The view controller that presented the view controller or that presented its farthest ancestor view controller.

