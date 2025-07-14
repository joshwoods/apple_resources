

- UIKit
- UIViewController
-  toolbarItems 

Instance Property

# toolbarItems

The toolbar items associated with the view controller.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var toolbarItems: [UIBarButtonItem]? { get set }
```

## Discussion

This property contains an array of UIBarButtonItem objects and works in conjunction with a UINavigationController object. If this view controller is embedded inside a navigation controller interface, and the navigation controller displays a toolbar, this property identifies the items to display in that toolbar.

You can set the value of this property explicitly or use the setToolbarItems(_:animated:) method to animate changes to the visible set of toolbar items.

## See Also

### Configuring a navigation interface

var navigationItem: UINavigationItem

The navigation item used to represent the view controller in a parent’s navigation bar.

var hidesBottomBarWhenPushed: Bool

A Boolean value indicating whether the toolbar at the bottom of the screen is hidden when the view controller is pushed on to a navigation controller.

func setToolbarItems([UIBarButtonItem]?, animated: Bool)

Sets the toolbar items to be displayed along with the view controller.

