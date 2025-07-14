

- UIKit
- UITabBarController
- UITabBarController.Sidebar
-  UITabBarController.Sidebar.Delegate 

Protocol

# UITabBarController.Sidebar.Delegate

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@MainActor
protocol Delegate : NSObjectProtocol
```

## Mentioned in 

Elevating your iPad app with a tab bar and sidebar

## Topics

### Instance Methods

func tabBarController(UITabBarController, sidebar: UITabBarController.Sidebar, contextMenuConfigurationFor: UITab) -> UIContextMenuConfiguration?

func tabBarController(UITabBarController, sidebar: UITabBarController.Sidebar, didEndDisplaying: UITab)

func tabBarController(UITabBarController, sidebar: UITabBarController.Sidebar, itemFor: UITabSidebarItem.Request) -> UITabSidebarItem

func tabBarController(UITabBarController, sidebar: UITabBarController.Sidebar, itemsForAddingTo: any UIDragSession, tab: UITab) -> [UIDragItem]

Called when a new drag session is requesting items to add to the existing drag session in the sidebar from the specified `tab`. Return items if the specified tab can add to the drag session, or an empty array if nothing should be added.

func tabBarController(UITabBarController, sidebar: UITabBarController.Sidebar, itemsForBeginning: any UIDragSession, tab: UITab) -> [UIDragItem]

Called when a new drag session has begun in the sidebar from the specified `tab`. Return drag items if the specified tab can be dragged, or an empty array if no drags should begin. Note that if drag items are returned on tabs in groups that allow reordering, then tab reordering is disabled when the sidebar is not in editing.

func tabBarController(UITabBarController, sidebar: UITabBarController.Sidebar, leadingSwipeActionsConfigurationFor: UITab) -> UISwipeActionsConfiguration?

func tabBarController(UITabBarController, sidebar: UITabBarController.Sidebar, sidebarAction: UIAction, group: UITabGroup, acceptItemsFrom: any UIDropSession)

Receive the drop from into the `sidebarAction` using the specified session. This is only called if the drop operation returned from `tabBarController:sidebar:sidebarAction:operationForAcceptingItemsFromDropSession` is valid for a drop.

func tabBarController(UITabBarController, sidebar: UITabBarController.Sidebar, sidebarAction: UIAction, group: UITabGroup, operationForAcceptingItemsFrom: any UIDropSession) -> UIDropOperation

Determines if items from the specified drop session can be dropped into the specified `sidebarAction`. If the operation is either a `.move` or `.copy`, then the drop will proceed and `tabBarController:sidebar:sidebarAction:acceptItemsFromDropSession:` is called. By default, the drop will be treated as a cancel operation if this is not implemented.

func tabBarController(UITabBarController, sidebar: UITabBarController.Sidebar, trailingSwipeActionsConfigurationFor: UITab) -> UISwipeActionsConfiguration?

func tabBarController(UITabBarController, sidebar: UITabBarController.Sidebar, update: UITabSidebarItem)

func tabBarController(UITabBarController, sidebar: UITabBarController.Sidebar, willBeginDisplaying: UITab)

func tabBarController(UITabBarController, sidebarVisibilityWillChange: UITabBarController.Sidebar, animator: any UITabBarController.Sidebar.Animating)

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting the sidebar delegate

var delegate: (any UITabBarController.Sidebar.Delegate)?

