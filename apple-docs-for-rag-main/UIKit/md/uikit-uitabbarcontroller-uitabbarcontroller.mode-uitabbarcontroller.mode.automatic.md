

- UIKit
- UITabBarController
- UITabBarController.Mode
-  UITabBarController.Mode.automatic 

Case

# UITabBarController.Mode.automatic

The system sets the display mode based on the tab’s content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
case automatic
```

## Discussion

Different platforms handle the mode differently:

- On iPad, If the tabs array contains one or more UITabGroup items, the system displays the content as either a tab bar or a sidebar, depending on the context. Otherwise, it only displays the content only as a tab bar.

- On Mac Catalyst, the system displays a sidebar if the tabs array contains one or more UITabGroup items. Otherwise, it displays a tab bar.

- On iPhone and Apple TV, the system displays the platform’s regular tab bar.

- In visionOS, the system displays the platform’s regular tabs, but a UITabGroup can display a sidebar when it displays the group’s view controller.

For more information, see Elevating your iPad app with a tab bar and sidebar.

## See Also

### Setting modes

case tabBar

The system displays the content only as a tab bar.

case tabSidebar

The system displays the content as either a tab bar or a sidebar, depending on the context.

