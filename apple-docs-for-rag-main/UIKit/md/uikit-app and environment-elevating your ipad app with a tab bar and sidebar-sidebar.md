

- UIKit
- App and environment
-  Elevating your iPad app with a tab bar and sidebar 

Article

# Elevating your iPad app with a tab bar and sidebar

Provide a compact, ergonomic tab bar for quick access to key parts of your app, and a sidebar for in-depth navigation.

## Overview

In iPadOS 18 and later, the position of the tab bar moves from the bottom of the screen to float over your content at the top. This compact appearance gives you more space for your app’s content. Additionally, because it shares space with the navigation bar, it places your tabs closer to your app’s other controls.

iPadOS apps automatically receive the new tab bar appearance when you compile them for iPadOS 18 and later.

SwiftUI equivalent

For information about adopting the new tab bar appearance in SwiftUI, read Enhancing your app’s content with tab navigation.

### Create a tab bar

iPadOS 18 also introduces new API for creating tab bars. Create a UITabBarController and assign an array of UITab objects to its tabs property. To create a tab, call init(title:image:identifier:viewControllerProvider:). In the closure, return the view controller your app presents when someone selects the tab. If you use SF Symbols for your tab’s image, be sure to select the outline variant. The system automatically selects the correct variant (outline or filled) based on the context. Additionally, you can change a tab’s properties, such as title or image, at runtime, and the system automatically updates its appearance.

```
// Create the tab bar controller.
let tabBarController = UITabBarController()

// Assign an array of tabs.
tabBarController.tabs = [

   UITab(title: "First",
         image: UIImage(systemName: "1.circle"),
         identifier: "First Tab") { _ in
             // Return the view controller that the tab displays.
             MyFirstViewController()
         },

   UITab(title: "Second",
         image: UIImage(systemName: "2.circle"),
         identifier: "Second Tab") { _ in
             // Return the view controller that the tab displays.
             MySecondViewController()
         },

   UITab(title: "Third",
         image: UIImage(systemName: "3.circle"),
         identifier: "Third Tab") { _ in
             // Return the view controller that the tab displays.
             MyThirdViewController()
         }
]
```

To add a search tab, create a UISearchTab instance and add it to the tabs array.

```
// Create a search tab.
UISearchTab { _ in 
    // Return the view controller that the tab displays.
    UINavigationController(
        rootViewController: MySearchViewController()
    )
}

```

The new iPad tab bar supports an unlimited number of items. If there isn’t enough room to display all the tabs, the system collapses any tabs that can’t fit onscreen, and lets people scroll through them. However, consider limiting your tabs to just those that fit in the tab bar. This ensures that people can access key parts of your app with one tap.

### Integrate the tab bar and sidebar

Although both tab bars and sidebars play a similar navigation role in iPadOS apps, they have different strengths. A tab bar is always available and represents the key parts of your app. A sidebar provides a richer collection of possible destinations; however, people typically need to navigate back to the sidebar to select a different option.

If your app contains a rich hierarchy of views, you can create an array of tab items that the system displays as either a tab bar or a sidebar. This combination provides the best features of both navigation styles. When displaying as a tab bar, people have quick access to the most critical sections of your app. When displaying as a sidebar, they can see the full range and depth of your app.

Use the new UITab and UITabGroup classes to create a hierarchy of tabs. If the tabs array contains at least one tab group, the system automatically displays the tabs as both a tab bar and a sidebar. Otherwise, it only displays the array as a tab bar. You can also explicitly define how the system displays your tabs by setting the UITabBarController object’s mode property.

```
// Enable the sidebar.
tabBarController.mode = .tabSidebar

// Get the sidebar.
let sidebar = tabBarController.sidebar

// Show the sidebar.
sidebar.isHidden = false
```

By default, the system presents the sidebar in landscape orientation and hides it in portrait orientation; however, people can toggle between the tab bar and sidebar in either orientation. You can also programmatically show and hide the sidebar by setting its isHidden property.

### Build a hierarchy of items for the sidebar

You can use UITabGroup to define a section of items in the sidebar. Provide an array of tabs for the section’s content and a view controller to display when someone selects the section from the tab bar.

```
let sectionOne = UITabGroup(
    title: "Section 1",
    image: UIImage(systemName: "1.square.fill"),
    identifier: "Section one",
    children:
        [
            UITab(
                title: "Subitem A",
                image: UIImage(systemName: "a.circle"),
                identifier: "Section 1, item A"
            ) { _ in
                MyFirstSubitemTabViewController()
            },

            UITab(
                title: "Subitem B",
                image: UIImage(systemName: "b.circle"),
                identifier: "Section 1, item b"
            ) { _ in
                MySecondSubitemTabViewController()
            },

            UITab(
                title: "Subitem C",
                image: UIImage(systemName: "c.circle"),
                identifier: "Section 1, item C"
            ) { _ in
                MyThirdSubitemTabViewController()
            },
        ]) { _ in
            // Return a view controller that the system displays when someone selects the section in the tab bar.
            MySectionViewController()
        }
```

The tab bar displays a tab group as a single tab item, and the sidebar displays it as a section that contains subitems. The sidebar displays top-level tab items first, followed by the sections.

You can nest a UITabGroup inside another UITabGroup to create a deeper hierarchy in the sidebar; however, consider limiting your app to two, or at most three, layers. Also, you can dynamically change a tab group’s content at runtime by modifying its children property.

### Add actions to the sidebar

You can add actions to the sidebar by setting a tab group’s sidebarActions property. These actions function like buttons that you place inside the tab group.

```
// Create the action.
let refreshAction = UIAction(title: "Refresh", image: UIImage(systemName: "arrow.clockwise")) { _ in
    myAction()
}

// Assign the action.
sectionOne.sidebarActions = [refreshAction]
```

To support swipe actions or context menus, assign a delegate to your sidebar that adopts the UITabBarController.Sidebar.Delegate protocol, and implement the following optional methods:

- tabBarController(_:sidebar:leadingSwipeActionsConfigurationFor:)

- tabBarController(_:sidebar:trailingSwipeActionsConfigurationFor:)

- tabBarController(_:sidebar:contextMenuConfigurationFor:)

To support drag-and-drop operations, assign a delegate to your tab bar that adopts the UITabBarControllerDelegate protocol, and implement the tabBarController(_:tab:operationForAcceptingItemsFrom:) and tabBarController(_:tab:acceptItemsFrom:) methods.

### Enable customization

With the new tab bar and sidebar, people can customize the content in both. The system provides a button to put the bars into edit mode. While editing, people can:

- Drag items from the sidebar to the tab bar to add them to the tab bar.

- Drag items from the tab bar to remove them from the tab bar.

- Drag items to reorder them in the tab bar.

- Drag items to reorder them inside their tab group.

- Uncheck items in the sidebar to hide them. This also removes them from the tab bar.

The system automatically persists any customizations that someone makes to the bars. You can implement the tabBarController(_:displayOrderDidChangeFor:) and tabBarController(_:visibilityDidChangeFor:) delegate methods to receive notifications about the changes.

By default, only the top-level tabs appear in the tab bar. People can add or remove any tab in the sidebar, but can’t hide or reorder the items in it.

To control which items appear in the tab bar, and how people can customize them, set the UITab object’s preferredPlacement property. Conceptually, you can think of the tab bar as having three different regions:

- Fixed tabs appear on the leading edge of the tab bar.

- Default, optional, and movable tabs appear after the fixed tabs.

- Pinned tabs are always visible on the trailing edge, and only show the tab’s image.

When possible, make tabs customizable so that people can choose which ones to place in the tab bar. If you have any tabs that are central to your app, consider making them fixed tabs, so that people can’t remove or move them. Use pinned tabs for prominent items, like search. Also, because pinned tabs only display the tab icon, be sure to select an image that people recognize and can easily understand.

To create an item that appears in the sidebar, but that people can’t add to the tab bar, set the preferredPlacement property to UITab.Placement.sidebarOnly. To create an item that people can add to or remove from the sidebar, set its allowsHiding property to true. If someone removes an item from the sidebar, the system also removes it from the tab bar.

```
// Create the tab.
var customizeableItem = UITab(
        title: "Optional",
        image: UIImage(systemName: "questionmark.app"),
        identifier: "Optional Item"
) { _ in
    MyOptionalViewController()
}

// Let people add and remove this item in the sidebar.
customizeableItem.allowsHiding = true

// Set the item as hidden in the sidebar by default.
customizeableItem.isHiddenByDefault = true
```

To let people reorganize items within a tab group, set the group’s allowsReordering property to true.

```
sectionOne.allowsReordering = true
```

You can also programmatically set the order of items in a tab group using its displayOrderIdentifiers property. By default, the system sets the tab group’s order based on its children property.

Important

When someone customizes the tab bar or sidebar, the system persists those changes. The next time your app launches, it sets each tab’s isHidden and displayOrderIdentifiers properties to the customized values. The system assigns these values when it adds the tab to the UITabBarController. If your app programmatically sets the isHidden or displayOrderIdentifiers properties before adding the tabs, the customized values override the values your app assigns. If, however, you change the values after adding the tabs, your values override the customizations.

### Use the tab bar and sidebar on other platforms

The new UITab API is also available in iOS 18, Mac Catalyst 18, tvOS 18, and visionOS 2, and later. Consider using this API to create tab bars on all UIKit-based projects.

The new tab bar and sidebar only appear on iPad. On iPhone and Apple TV, the system displays the platform’s regular tab bar. For Mac Catalyst, it displays a tab bar if the tab bar controller’s mode property is UITabBarController.Mode.tabBar, and a sidebar if it’s UITabBarController.Mode.tabSidebar.

In visionOS, the system displays the platform’s regular tabs, but a UITabGroup can display a sidebar when it displays the group’s view controller.

## See Also

### iPad

Building a desktop-class iPad app

Optimize your iPad app’s user experience by adopting desktop-class enhancements for multitasking with Stage Manager, document interactions, text editing, search, and more.

Supporting desktop-class features in your iPad app

Enhance your iPad app by adding desktop-class features and document support.

Multitasking on iPad

Implement multitasking APIs to seamlessly integrate your app with iPadOS.

