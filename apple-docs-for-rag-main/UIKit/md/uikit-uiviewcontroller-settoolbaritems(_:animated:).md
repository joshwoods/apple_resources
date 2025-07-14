

- UIKit
- UIViewController
-  setToolbarItems(\_:animated:) 

Instance Method

# setToolbarItems(\_:animated:)

Sets the toolbar items to be displayed along with the view controller.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setToolbarItems(
    _ toolbarItems: [UIBarButtonItem]?,
    animated: Bool
)
```

## Parameters 

`toolbarItems`  

The toolbar items to display in a built-in toolbar.

`animated`  

If true, animate the change of items in the toolbar.

## Discussion

View controllers that are managed by a navigation controller can use this method to specify toolbar items for the navigation controller’s built-in toolbar. You can set the toolbar items for your view controller before your view controller is displayed or after it is already visible.

## See Also

### Configuring a navigation interface

var navigationItem: UINavigationItem

The navigation item used to represent the view controller in a parent’s navigation bar.

var hidesBottomBarWhenPushed: Bool

A Boolean value indicating whether the toolbar at the bottom of the screen is hidden when the view controller is pushed on to a navigation controller.

var toolbarItems: [UIBarButtonItem]?

The toolbar items associated with the view controller.

