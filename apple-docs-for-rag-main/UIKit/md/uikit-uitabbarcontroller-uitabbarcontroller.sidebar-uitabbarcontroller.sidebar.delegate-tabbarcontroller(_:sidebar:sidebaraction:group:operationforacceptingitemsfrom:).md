

- UIKit
- UITabBarController
- UITabBarController.Sidebar
- UITabBarController.Sidebar.Delegate
-  tabBarController(\_:sidebar:sidebarAction:group:operationForAcceptingItemsFrom:) 

Instance Method

# tabBarController(\_:sidebar:sidebarAction:group:operationForAcceptingItemsFrom:)

Determines if items from the specified drop session can be dropped into the specified `sidebarAction`. If the operation is either a `.move` or `.copy`, then the drop will proceed and `tabBarController:sidebar:sidebarAction:acceptItemsFromDropSession:` is called. By default, the drop will be treated as a cancel operation if this is not implemented.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
@MainActor
optional func tabBarController(
    _ tabBarController: UITabBarController,
    sidebar: UITabBarController.Sidebar,
    sidebarAction: UIAction,
    group: UITabGroup,
    operationForAcceptingItemsFrom session: any UIDropSession
) -> UIDropOperation
```

