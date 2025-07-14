

- UIKit
- UINavigationController
-  toolbar 

Instance Property

# toolbar

The custom toolbar associated with the navigation controller.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var toolbar: UIToolbar! { get }
```

## Discussion

This property contains a reference to the built-in toolbar managed by the navigation controller. Access to this toolbar is provided solely for clients that want to present an action sheet from the toolbar. You should not modify the UIToolbar object directly.

Management of this toolbar’s contents is done through the custom view controllers associated with this navigation controller. For each view controller on the navigation stack, you can assign a custom set of toolbar items using the setToolbarItems(_:animated:) method of UIViewController.

The visibility of this toolbar is controlled by the isToolbarHidden property. The toolbar also obeys the hidesBottomBarWhenPushed property of the currently visible view controller and hides and shows itself automatically as needed.

## See Also

### Configuring custom toolbars

func setToolbarHidden(Bool, animated: Bool)

Changes the visibility of the navigation controller’s built-in toolbar.

var isToolbarHidden: Bool

A Boolean indicating whether the navigation controller’s built-in toolbar is visible.

class let hideShowBarDuration: CGFloat

A variable that specifies the duration when animating the navigation bar.

