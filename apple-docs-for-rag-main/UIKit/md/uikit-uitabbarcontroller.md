

- UIKit
-  UITabBarController 

Class

# UITabBarController

A container view controller that manages a multiselection interface, where the selection determines which child view controller to display.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UITabBarController
```

## Mentioned in 

Elevating your iPad app with a tab bar and sidebar

Managing content in your app’s windows

Creating a custom container view controller

## Overview

The tab bar interface displays tabs at the bottom of the window for selecting between the different modes and for displaying the views for that mode. This class is generally used as-is, but may also be subclassed.

Each tab of a tab bar controller interface is associated with a custom view controller. When the user selects a specific tab, the tab bar controller displays the root view of the corresponding view controller, replacing any previous views. (User taps always display the root view of the tab, regardless of which tab was previously selected. This is true even if the tab was already selected.) Because selecting a tab replaces the contents of the interface, the type of interface managed in each tab need not be similar in any way. In fact, tab bar interfaces are commonly used either to present different types of information or to present the same information using a completely different style of interface. The following image shows the tab bar interface presented by the Clock app, each tab of which presents a type of time based information.

You should never access the tab bar view of a tab bar controller directly. To configure the tabs of a tab bar controller, you assign the view controllers that provide the root view for each tab to the viewControllers property. The order in which you specify the view controllers determines the order in which they appear in the tab bar. When setting this property, you should also assign a value to the selectedViewController property to indicate which view controller is selected initially. (You can also select view controllers by array index using the selectedIndex property.) When you embed the tab bar controller’s view (obtained using the inherited view property) in your app window, the tab bar controller automatically selects that view controller and displays its contents, resizing them as needed to fit the tab bar interface.

Tab bar items are configured through their corresponding view controller. To associate a tab bar item with a view controller, create a new instance of the UITabBarItem class, configure it appropriately for the view controller, and assign it to the view controller’s tabBarItem property. If you don’t provide a custom tab bar item for your view controller, the view controller creates a default item containing no image and the text from the view controller’s title property.

As the user interacts with a tab bar interface, the tab bar controller object sends notifications about the interactions to its delegate. The delegate can be any object you specify but must conform to the UITabBarControllerDelegate protocol. You can use the delegate to prevent specific tab bar items from being selected and to perform additional tasks when tabs are selected. You can also use the delegate to monitor changes to the tab bar that are made by the More navigation controller, which is described in more detail in The More navigation controller.

### The views of a tab bar controller

Because the UITabBarController class inherits from the UIViewController class, tab bar controllers have their own view that’s accessible through the view property. The view for a tab bar controller is just a container for a tab bar view and the view containing your custom content. The tab bar view provides the selection controls for the user and consists of one or more tab bar items. The following image shows how these views are assembled to present the overall tab bar interface. Although the items in the tab bar and toolbar views can change, the views that manage them don’t. Only the custom content view changes to reflect the view controller for the currently selected tab.

You can use navigation controllers or custom view controllers as the root view controller for a tab. If the root view controller is a navigation controller, the tab bar controller makes further adjustments to the size of the displayed navigation content so that it doesn’t overlap the tab bar. Any views you display in a tab bar interface should therefore have their autoresizingMask property set to resize the view appropriately under any conditions.

### The More navigation controller

The tab bar has limited space for displaying your custom items. If you add six or more custom view controllers to a tab bar controller, the tab bar controller displays only the first four items plus the standard More item on the tab bar. Tapping the More item brings up a standard interface for selecting the remaining items.

The interface for the standard More item includes an Edit button that allows the user to reconfigure the tab bar. By default, the user is allowed to rearrange all items on the tab bar. If you do not want the user to modify some items, though, you can remove the appropriate view controllers from the array in the customizableViewControllers property.

Note

Tab bar customization and the More interface are not available in tvOS.

### State preservation

In iOS 6 and later, if you assign a value to this view controller’s restorationIdentifier property, it preserves a reference to the view controller in the selected tab. At restore time, it uses the reference to select the tab with the same view controller.

When preserving a tab bar controller, assign unique restoration identifiers to the child view controllers you want to preserve. Omitting a restoration identifier from a child view controller causes that tab to return to its default configuration. Although the tab bar controller saves its tabs in the same order that they are listed in the viewControllers property, the save order is actually irrelevant. Your code is responsible for providing the new tab bar controller during the next launch cycle, so your code can adjust the order of the tabs as needed. The state preservation system restores the contents of each tab based on the assigned restoration identifier, not based on the position of the tab.

For more information about how state preservation and restoration works, see App Programming Guide for iOS.

### Differences between iOS and tvOS

Tab bar controllers serve the same purpose in tvOS as in iOS, but provide slightly different user interface features:

- In tvOS, the tab bar interface appears at the top of the window. When focus leaves the tab bar, the tab bar remains fixed at the top of the screen by default. To create an interface where the tab bar doesn’t remain fixed, but instead scrolls with the content, set the tabBarObservedScrollView property to the appropriate scroll view. In iOS, the tab bar always stays pinned at the bottom of the screen.

- In tvOS, swiping down from the tab bar moves focus into the content view; specifically, to the first focusable view that’s visually below the selected tab. Swiping down behaves like a normal focus-changing gesture — that is, focus moves in the direction the user swiped. If nothing is focusable immediately below the selected tab, the closest focusable view is focused instead. In iOS, the tab bar always remains in focus at the bottom of the screen.

- In tvOS, pressing the Select button while a tab is focused moves focus into the content view. Because there’s no direction associated with this change, focus moves to the most appropriate view specified in the content view’s preferredFocusEnvironments property. In iOS, there’s no notion of focusing between views.

- Tab bar controllers in tvOS don’t support customization. A tab bar controller displays only the number of view controllers from its viewControllers array that fit on the screen, and doesn’t provide the More interface seen in iOS.

## Topics

### Assigning tabs

var tabs: [UITab]

An array of tabs that the tab bar displays.

### Supporting the sidebar

var mode: UITabBarController.Mode

The display mode for a tab bar.

enum Mode

A tab bar’s display mode.

var sidebar: UITabBarController.Sidebar

A tab bar’s corresponding sidebar.

class Sidebar

An object for managing and configuring the sidebar.

class UITabSidebarItem

class Request

protocol Animating

### Customizing the tab bar behavior

var delegate: (any UITabBarControllerDelegate)?

The tab bar controller’s delegate object.

protocol UITabBarControllerDelegate

A set of methods you implement to customize the behavior of a tab bar.

### Accessing the tab bar controller properties

var tabBar: UITabBar

The tab bar view associated with this controller.

### Managing the view controllers

var viewControllers: [UIViewController]?

An array of the root view controllers displayed by the tab bar interface.

func setViewControllers([UIViewController]?, animated: Bool)

Sets the root view controllers of the tab bar controller.

var customizableViewControllers: [UIViewController]?

The subset of view controllers managed by this tab bar controller that can be customized.

var moreNavigationController: UINavigationController

The view controller that manages the More navigation interface.

### Managing the selected tab

var selectedViewController: UIViewController?

The view controller associated with the currently selected tab item.

var selectedIndex: Int

The index of the view controller associated with the currently selected tab item.

### Initializers

init(tabs: [UITab])

### Instance Properties

var compactTabIdentifiers: [String]?

var customizationIdentifier: String?

var isTabBarHidden: Bool

var selectedTab: UITab?

### Instance Methods

func setTabBarHidden(Bool, animated: Bool)

func setTabs([UITab], animated: Bool)

func tab(forIdentifier: String) -> UITab?

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITabBarDelegate
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Container view controllers

Creating a custom container view controller

Create a composite interface by combining content from one or more view controllers with other custom views.

class UISplitViewController

A container view controller that implements a hierarchical interface.

class UINavigationController

A container view controller that defines a stack-based scheme for navigating hierarchical content.

class UINavigationBar

Navigational controls that display in a bar along the top of the screen, usually in conjunction with a navigation controller.

class UINavigationItem

The items that a navigation bar displays when the associated view controller is visible.

class UITabBar

A control that displays one or more buttons in a tab bar for selecting between different subtasks, views, or modes in an app.

class UITabBarItem

An object that describes an item in a tab bar.

class UITab

An object that manages a tab in a tab bar.

class UISearchTab

A tab subclass that represents the system’s search tab.

class UITabGroup

An object that manages a collection of tab objects.

class UIPageViewController

A container view controller that manages navigation between pages of content, where a subview controller manages each page.

