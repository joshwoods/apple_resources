

- UIKit
- UITabBarController
- UITabBarController.Sidebar
- UITabBarController.Sidebar.Delegate
-  tabBarController(\_:sidebar:sidebarAction:group:acceptItemsFrom:) 

Instance Method

# tabBarController(\_:sidebar:sidebarAction:group:acceptItemsFrom:)

Receive the drop from into the `sidebarAction` using the specified session. This is only called if the drop operation returned from `tabBarController:sidebar:sidebarAction:operationForAcceptingItemsFromDropSession` is valid for a drop.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
@MainActor
optional func tabBarController(
    _ tabBarController: UITabBarController,
    sidebar: UITabBarController.Sidebar,
    sidebarAction: UIAction,
    group: UITabGroup,
    acceptItemsFrom session: any UIDropSession
)
```

