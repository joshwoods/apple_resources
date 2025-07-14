

- AppKit
- NSSplitViewItem
-  viewController 

Instance Property

# viewController

The view controller that the split view item represents.

macOS 10.10+

``` source
var viewController: NSViewController { get set }
```

## Discussion

Don’t set this property while adding the split view item to a split view controller. If you do, the system raises an exception.

