

- UIKit
- UISplitViewController
-  setViewController(\_:for:) 

Instance Method

# setViewController(\_:for:)

Presents the provided view controller in the specified column of the split view interface.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
func setViewController(
    _ vc: UIViewController?,
    for column: UISplitViewController.Column
)
```

## Parameters 

`vc`  

The child view controller to associate with the provided column of the split view interface.

`column`  

The corresponding column of the split view interface. See UISplitViewController.Column for values.

## Discussion

This method doesn’t apply to classic split view controllers with a style of UISplitViewController.Style.unspecified. For a classic split view controller, instead use the viewControllers property to assign the primary and secondary view controllers that you want to display initially. After the split view controller is onscreen, set the child view controllers using the show(_:sender:) and showDetailViewController(_:sender:) methods.

For a column-style split view controller, you use this method to assign child view controllers to a specific column of the split view interface. In general, unless your view controller is a navigation controller, the split view creates its own navigation controller to wrap the view controller you assign to the primary, supplementary, and secondary columns. There are some exceptions to this behavior:

- For the primary column, if you assign a UIViewController (or custom subclass) whose first child view controller is a UINavigationController, the split view controller uses that navigation controller as the primary view controller for collapsing the interface and for placing the button to change the display mode.

- For the secondary column, if you assign a UIViewController (or custom subclass) whose first child view controller is a UINavigationController, the split view controller uses that navigation controller as the secondary view controller for placing the button to change the display mode.

| Column | Assigned As-Is |
|----|----|
| Primary | UINavigationController  UIViewController with UINavigationController as its first child |
| Supplementary | UINavigationController |
| Secondary | UITabBarController with UINavigationControllers in its tabs  UINavigationController  UIViewController with UINavigationController as its first child |
| Compact | Any UIViewController |

You can’t assign a UITabBarController to the primary or supplementary columns.

## See Also

### Managing the child view controllers

enum Column

Constants that describe the columns within the split view interface.

func viewController(for: UISplitViewController.Column) -> UIViewController?

Returns the view controller associated with the specified column of the split view interface.

var viewControllers: [UIViewController]

The array of view controllers the split view controller manages.

