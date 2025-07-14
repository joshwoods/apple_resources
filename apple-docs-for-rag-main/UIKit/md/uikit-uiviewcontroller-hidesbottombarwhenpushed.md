

- UIKit
- UIViewController
-  hidesBottomBarWhenPushed 

Instance Property

# hidesBottomBarWhenPushed

A Boolean value indicating whether the toolbar at the bottom of the screen is hidden when the view controller is pushed on to a navigation controller.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
var hidesBottomBarWhenPushed: Bool { get set }
```

## Discussion

A view controller added as a child of a navigation controller can display an optional toolbar at the bottom of the screen. The value of this property on the topmost view controller determines whether the toolbar is visible. If the value of this property is true, the toolbar is hidden. If the value of this property is false, the bar is visible.

## See Also

### Configuring a navigation interface

var navigationItem: UINavigationItem

The navigation item used to represent the view controller in a parent’s navigation bar.

func setToolbarItems([UIBarButtonItem]?, animated: Bool)

Sets the toolbar items to be displayed along with the view controller.

var toolbarItems: [UIBarButtonItem]?

The toolbar items associated with the view controller.

