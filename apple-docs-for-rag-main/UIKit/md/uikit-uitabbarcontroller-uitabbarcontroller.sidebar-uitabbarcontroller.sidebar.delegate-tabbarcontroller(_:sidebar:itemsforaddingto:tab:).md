

- UIKit
- UITabBarController
- UITabBarController.Sidebar
- UITabBarController.Sidebar.Delegate
-  tabBarController(\_:sidebar:itemsForAddingTo:tab:) 

Instance Method

# tabBarController(\_:sidebar:itemsForAddingTo:tab:)

Called when a new drag session is requesting items to add to the existing drag session in the sidebar from the specified `tab`. Return items if the specified tab can add to the drag session, or an empty array if nothing should be added.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
@MainActor
optional func tabBarController(
    _ tabBarController: UITabBarController,
    sidebar: UITabBarController.Sidebar,
    itemsForAddingTo dragSession: any UIDragSession,
    tab: UITab
) -> [UIDragItem]
```

