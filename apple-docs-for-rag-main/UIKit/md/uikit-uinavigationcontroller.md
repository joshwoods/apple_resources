

- UIKit
-  UINavigationController 

Class

# UINavigationController

A container view controller that defines a stack-based scheme for navigating hierarchical content.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UINavigationController
```

## Mentioned in 

Managing content in your app’s windows

Creating a custom container view controller

Customizing the behavior of segue-based presentations

Displaying and managing views with a view controller

## Overview

A navigation controller is a container view controller that manages one or more child view controllers in a navigation interface. In this type of interface, only one child view controller is visible at a time. Selecting an item in the view controller pushes a new view controller onscreen using an animation, hiding the previous view controller. Tapping the back button in the navigation bar at the top of the interface removes the top view controller, thereby revealing the view controller underneath.

Use a navigation interface to mimic the organization of hierarchical data managed by your app. At each level of the hierarchy, you provide an appropriate screen (managed by a custom view controller) to display the content at that level. The following image shows an example of the navigation interface presented by the Settings application in iOS Simulator. The first screen presents the user with the list of applications that contain preferences. Selecting an application reveals individual settings and groups of settings for that application. Selecting a group yields more settings and so on. For all but the root view, the navigation controller provides a back button to allow the user to move back up the hierarchy.

A navigation controller object manages its child view controllers using an ordered array, known as the *navigation stack*. The first view controller in the array is the root view controller and represents the bottom of the stack. The last view controller in the array is the topmost item on the stack, and represents the view controller currently being displayed. You add and remove view controllers from the stack using segues or using the methods of this class. The user can also remove the topmost view controller using the back button in the navigation bar or using a left-edge swipe gesture.

The navigation controller manages the navigation bar at the top of the interface and an optional toolbar at the bottom of the interface. The navigation bar is always present and is managed by the navigation controller itself, which updates the navigation bar using the content provided by its child view controllers. When the isToolbarHidden property is false, the navigation controller similarly updates the toolbar with contents provided by the topmost view controller.

A navigation controller coordinates its behavior with its delegate object. The delegate object can override the pushing or popping of view controllers, provide custom animation transitions, and specify the preferred orientation for the navigation interface. The delegate object you provide must conform to the UINavigationControllerDelegate protocol.

The following image shows the relationships between the navigation controller and the objects it manages. Use the specified properties of the navigation controller to access these objects.

### Navigation controller views

A navigation controller is a container view controller — that is, it embeds the content of other view controllers inside of itself. You access a navigation controller’s view from its view property. This view incorporates the navigation bar, an optional toolbar, and the content view corresponding to the topmost view controller. The following image shows how these views are assembled to present the overall navigation interface. (In this figure, the navigation interface is further embedded inside a tab bar interface.) Although the content of the navigation bar and toolbar views changes, the views themselves don’t. The only view that actually changes is the custom content view provided by the topmost view controller on the navigation stack.

Note

Because the content view underlaps the navigation bar in iOS 7 and later, you must consider that space when designing your view controller content.

The navigation controller manages the creation, configuration, and display of the navigation bar and optional navigation toolbar. It’s permissible to customize the navigation bar’s appearance-related properties but you must never change its frame, bounds, or alpha values directly. If you subclass UINavigationBar, you must initialize your navigation controller using the init(navigationBarClass:toolbarClass:) method. To hide or show the navigation bar, use the isNavigationBarHidden property or setNavigationBarHidden(_:animated:) method.

A navigation controller builds the contents of the navigation bar dynamically using the navigation item objects (instances of the UINavigationItem class) associated with the view controllers on the navigation stack. To customize the overall appearance of a navigation bar, use UIAppearance APIs. To change the contents of the navigation bar, you must therefore configure the navigation items of your custom view controllers. For more information about navigation items, see UINavigationItem.

### Updating the navigation bar

Each time the top-level view controller changes, the navigation controller updates the navigation bar accordingly. Specifically, the navigation controller updates the bar button items displayed in each of the three navigation bar positions: left, middle, and right. Bar button items are instances of the UIBarButtonItem class. You can create items with custom content or create standard system items depending on your needs.

Tinting of the navigation bar is controlled by properties of the navigation bar itself. Use the tintColor property to change the tint color of items in the bar and use the barTintColor property to change the tint color of the bar itself. Navigation bars don’t inherit their tint color from the currently displayed view controller.

For more information about the navigation bar, see UINavigationBar. For more information about how to create bar button items, see UIBarButtonItem.

#### The left item

For all but the root view controller on the navigation stack, the item on the left side of the navigation bar provides navigation back to the previous view controller. The contents of this left-most button are determined as follows:

- If the new top-level view controller has a custom left bar button item, that item is displayed. To specify a custom left bar button item, set the leftBarButtonItem property of the view controller’s navigation item.

- If the top-level view controller doesn’t have a custom left bar button item, but the navigation item of the previous view controller has an object in its backBarButtonItem property, the navigation bar displays that item.

- If a custom bar button item isn’t specified by either of the view controllers, a default back button is used and its title is set to the value of the title property of the previous view controller — that is, the view controller one level down on the stack. (If there’s only one view controller on the navigation stack, no back button is displayed.)

Note

In cases where the title of a back button is too long to fit in the available space, the navigation bar may substitute the string “Back” for the actual button title. The navigation bar does this only if the back button is provided by the previous view controller. If the new top-level view controller has a custom left bar button item — an object in the leftBarButtonItem or leftBarButtonItems property of its navigation item—the navigation bar doesn’t change the button title.

#### The middle item

The navigation controller updates the middle of the navigation bar as follows:

- If the new top-level view controller has a custom title view, the navigation bar displays that view in place of the default title view. To specify a custom title view, set the titleView property of the view controller’s navigation item.

- If no custom title view is set, the navigation bar displays a label containing the view controller’s default title. The string for this label is usually obtained from the title property of the view controller itself. If you want to display a different title than the one associated with the view controller, set the title property of the view controller’s navigation item instead.

#### The right item

The navigation controller updates the right side of the navigation bar as follows:

- If the new top-level view controller has a custom right bar button item, that item is displayed. To specify a custom right bar button item, set the rightBarButtonItem property of the view controller’s navigation item.

- If no custom right bar button item is specified, the navigation bar displays nothing on the right side of the bar.

### Displaying a toolbar

A navigation controller object manages an optional toolbar in its view hierarchy. When displayed, this toolbar obtains its current set of items from the toolbarItems property of the active view controller. When the active view controller changes, the navigation controller updates the toolbar items to match the new view controller, animating the new items into position when appropriate.

The navigation toolbar is hidden by default but you can show it for your navigation interface by calling the setToolbarHidden(_:animated:) method of your navigation controller object. If not all of your view controllers support toolbar items, your delegate object can call this method to toggle the visibility of the toolbar during subsequent push and pop operations. To use a custom UIToolbar subclass, initialize the navigation controller using the init(navigationBarClass:toolbarClass:) method. If you use custom toolbar and navigation bar subclasses to create a navigation controller, note that you’re responsible for pushing and setting view controllers before presenting the navigation controller onscreen.

### Adapting to different environments

The navigation interface remains the same in both horizontally compact and horizontally regular environments. When toggling between the two environments, only the size of the navigation controller’s view changes. The navigation controller doesn’t change its view hierarchy or the layout of its views.

When configuring segues between view controllers on a navigation stack, the standard Show and Show Detail segues behave as follows:

Show segue  
The navigation controller pushes the specified view controller onto its navigation stack.

Show Detail segue  
The navigation controller presents the specified view controller modally.

The behaviors of other segue types are unchanged.

### Interface behaviors

A navigation controller supports the following behaviors for its interface:

Supported interface orientations  
A navigation controller object doesn’t consult the view controllers on its navigation stack when determining the supported interface orientations. On iPhone, a navigation controller supports all orientations except portrait upside-down. On iPad, a navigation controller supports all orientations. If the navigation controller has a delegate object, the delegate can specify a different set of supported orientations using the navigationControllerSupportedInterfaceOrientations(_:) method.

Presentation context  
A navigation controller defines the presentation context for modally presented view controllers. When the modal transition style is UIModalPresentationStyle.currentContext or UIModalPresentationStyle.overCurrentContext, modal presentations from the view controllers in the navigation stack cover the entire navigation interface.

### State preservation

When you assign a value to a navigation controller’s restorationIdentifier property, it attempts to preserve itself and the child view controllers on its navigation stack. The navigation controller starts at the bottom of the stack and moves upward, encoding each view controller that also has a valid restoration identifier string. During the next launch cycle, the navigation controller restores the preserved view controllers to the navigation stack in the same order that they were preserved.

The child view controllers you push onto the navigation stack may use the same restoration identifiers. The navigation controller automatically stores additional information to ensure that each child’s restoration path is unique.

For more information about how state preservation and restoration works, see Preserving your app’s UI across launches.

## Topics

### Creating a navigation controller

init(rootViewController: UIViewController)

Initializes and returns a newly created navigation controller.

init(navigationBarClass: AnyClass?, toolbarClass: AnyClass?)

Initializes and returns a newly created navigation controller that uses your custom bar subclasses.

init(nibName: String?, bundle: Bundle?)

Creates a navigation controller with the nib file in the specified bundle.

init?(coder: NSCoder)

Creates a navigation controller from data in an unarchiver.

### Customizing the navigation interface behavior

var delegate: (any UINavigationControllerDelegate)?

The delegate of the navigation controller object.

protocol UINavigationControllerDelegate

The interface for an object that serves as a navigation controller’s delegate.

### Accessing items on the navigation stack

var topViewController: UIViewController?

The view controller at the top of the navigation stack.

var visibleViewController: UIViewController?

The view controller associated with the currently visible view in the navigation interface.

var viewControllers: [UIViewController]

The view controllers currently on the navigation stack.

func setViewControllers([UIViewController], animated: Bool)

Replaces the view controllers currently managed by the navigation controller with the specified items.

### Pushing and popping stack items

func pushViewController(UIViewController, animated: Bool)

Pushes a view controller onto the receiver’s stack and updates the display.

func popViewController(animated: Bool) -> UIViewController?

Pops the top view controller from the navigation stack and updates the display.

func popToRootViewController(animated: Bool) -> [UIViewController]?

Pops all the view controllers on the stack except the root view controller and updates the display.

func popToViewController(UIViewController, animated: Bool) -> [UIViewController]?

Pops view controllers until the specified view controller is at the top of the navigation stack.

var interactivePopGestureRecognizer: UIGestureRecognizer?

The gesture recognizer responsible for popping the top view controller off the navigation stack.

### Configuring navigation bars

var navigationBar: UINavigationBar

The navigation bar managed by the navigation controller.

func setNavigationBarHidden(Bool, animated: Bool)

Sets whether the navigation bar is hidden.

Customizing your app’s navigation bar

Create custom titles, prompts, and buttons in your app’s navigation bar.

### Configuring custom toolbars

var toolbar: UIToolbar!

The custom toolbar associated with the navigation controller.

func setToolbarHidden(Bool, animated: Bool)

Changes the visibility of the navigation controller’s built-in toolbar.

var isToolbarHidden: Bool

A Boolean indicating whether the navigation controller’s built-in toolbar is visible.

class let hideShowBarDuration: CGFloat

A variable that specifies the duration when animating the navigation bar.

### Hiding the navigation bar

var hidesBarsOnTap: Bool

A Boolean value indicating whether the navigation controller allows hiding of its bars using a tap gesture.

var hidesBarsOnSwipe: Bool

A Boolean value indicating whether the navigation bar hides its bars in response to a swipe gesture.

var hidesBarsWhenVerticallyCompact: Bool

A Boolean value indicating whether the navigation controller hides its bars in a vertically compact environment.

var hidesBarsWhenKeyboardAppears: Bool

A Boolean value indicating whether the navigation controller hides its bars when the keyboard appears.

var isNavigationBarHidden: Bool

A Boolean value that indicates whether the navigation bar is hidden.

var barHideOnTapGestureRecognizer: UITapGestureRecognizer

The gesture recognizer used to hide and show the navigation and toolbar.

var barHideOnSwipeGestureRecognizer: UIPanGestureRecognizer

The gesture recognizer used to hide the navigation bar and toolbar.

### Displaying view controllers

func show(UIViewController, sender: Any?)

Presents the specified view controller in the navigation interface.

## Relationships

### Inherits From

- UIViewController

### Inherited By

- UIImagePickerController
- UIVideoEditorController

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
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Container view controllers

Creating a custom container view controller

Create a composite interface by combining content from one or more view controllers with other custom views.

class UISplitViewController

A container view controller that implements a hierarchical interface.

class UINavigationBar

Navigational controls that display in a bar along the top of the screen, usually in conjunction with a navigation controller.

class UINavigationItem

The items that a navigation bar displays when the associated view controller is visible.

class UITabBarController

A container view controller that manages a multiselection interface, where the selection determines which child view controller to display.

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

