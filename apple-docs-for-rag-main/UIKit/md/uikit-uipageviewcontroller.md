

- UIKit
-  UIPageViewController 

Class

# UIPageViewController

A container view controller that manages navigation between pages of content, where a subview controller manages each page.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIPageViewController
```

## Mentioned in 

Managing content in your app’s windows

Creating a custom container view controller

## Overview

Page view controller–navigation can be controlled programmatically by your app or directly by the user using gestures. When navigating from page to page, the page view controller uses the transition that you specify to animate the change.

Important

In tvOS, the UIPageViewController class provides only a way to swipe between full-screen content pages. Unlike in iOS, a user cannot interact with or move focus between items on each page.

When defining a page view controller interface, you can provide the content view controllers one at a time (or two at a time, depending upon the spine position and double-sided state) or as-needed using a data source. When providing content view controllers one at a time, you use the setViewControllers(_:direction:animated:completion:) method to set the current content view controllers. To support gesture-based navigation, you must provide your view controllers using a data source object.

The data source for a page view controller is responsible for providing the content view controllers on demand and must conform to the UIPageViewControllerDataSource protocol. The delegate object—an object that conforms to the UIPageViewControllerDelegate protocol—provides some appearance-related information and receives notifications about gesture-initiated transitions.

This class is generally used as-is, but can also be subclassed.

## Topics

### Creating a page view controller

init(transitionStyle: UIPageViewController.TransitionStyle, navigationOrientation: UIPageViewController.NavigationOrientation, options: [UIPageViewController.OptionsKey : Any]?)

Initializes a newly created page view controller.

init?(coder: NSCoder)

Creates a page view controller from data in an unarchiver.

struct OptionsKey

Keys for creating the page view controller.

### Providing the Page Content

var dataSource: (any UIPageViewControllerDataSource)?

The object that provides view controllers.

protocol UIPageViewControllerDataSource

The UIPageViewControllerDataSource protocol is adopted by an object that provides view controllers to the page view controller on an as-needed basis, in response to navigation gestures.

### Customizing the Page View Behavior

var delegate: (any UIPageViewControllerDelegate)?

The delegate object.

protocol UIPageViewControllerDelegate

The delegate of a page view controller must adopt the UIPageViewControllerDelegate protocol. These methods allow the delegate to receive a notification when the device orientation changes and when the user navigates to a new page. For page-curl style transitions, the delegate can provide a different spine location in response to a change in the interface orientation.

### Providing Content

func setViewControllers([UIViewController]?, direction: UIPageViewController.NavigationDirection, animated: Bool, completion: ((Bool) -> Void)?)

Sets the view controllers to be displayed.

enum NavigationDirection

Directions for page-turn transitions.

var viewControllers: [UIViewController]?

The view controllers displayed by the page view controller.

var gestureRecognizers: [UIGestureRecognizer]

An array of UIGestureRecognizer objects that are configured to handle user interaction.

### Display Options

var navigationOrientation: UIPageViewController.NavigationOrientation

The direction along which navigation occurs.

enum NavigationOrientation

Orientations for page-turn transitions.

var spineLocation: UIPageViewController.SpineLocation

The location of the spine.

enum SpineLocation

Locations for the spine.

var transitionStyle: UIPageViewController.TransitionStyle

The style used to transition between view controllers.

enum TransitionStyle

Styles for the page-turn transition.

var isDoubleSided: Bool

A Boolean value that indicates whether content appears on the back of pages.

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

