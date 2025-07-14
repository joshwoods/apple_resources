

- AppKit
- NSCustomTouchBarItem
-  viewController 

Instance Property

# viewController

A view controller whose view is displayed in the bar to represent this item.

macOS 10.12.2+

``` source
@MainActor
var viewController: NSViewController? { get set }
```

## Discussion

When set, the item’s view property returns the view controller’s view property.

The property is automatically set to `nil` if you provide your own value for the view property.

## See Also

### Providing item content

var view: NSView

The view displayed in the bar to represent this item.

