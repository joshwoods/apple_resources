

- UIKit
- UITabBarController
- UITabBarController.Sidebar
- UITabBarController.Sidebar.Delegate
-  tabBarController(\_:sidebar:itemsForBeginning:tab:) 

Instance Method

# tabBarController(\_:sidebar:itemsForBeginning:tab:)

Called when a new drag session has begun in the sidebar from the specified `tab`. Return drag items if the specified tab can be dragged, or an empty array if no drags should begin. Note that if drag items are returned on tabs in groups that allow reordering, then tab reordering is disabled when the sidebar is not in editing.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
@MainActor
optional func tabBarController(
    _ tabBarController: UITabBarController,
    sidebar: UITabBarController.Sidebar,
    itemsForBeginning dragSession: any UIDragSession,
    tab: UITab
) -> [UIDragItem]
```

