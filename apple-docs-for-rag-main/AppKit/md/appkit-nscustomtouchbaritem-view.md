

- AppKit
- NSCustomTouchBarItem
-  view 

Instance Property

# view

The view displayed in the bar to represent this item.

macOS 10.12.2+

``` source
@MainActor
var view: NSView { get set }
```

## Discussion

By default, this property returns the value of view property from the view controller assigned to the viewController property.

If you set the value of this property, then the viewController property is automatically set to `nil`.

## See Also

### Providing item content

var viewController: NSViewController?

A view controller whose view is displayed in the bar to represent this item.

