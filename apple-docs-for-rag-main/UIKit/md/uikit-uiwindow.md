

- UIKit
-  UIWindow 

Class

# UIWindow

The backdrop for your app’s user interface and the object that dispatches events to your views.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIWindow
```

## Mentioned in 

Using responders and the responder chain to handle events

## Overview

Windows work with your view controllers to handle events and to perform many other tasks that are fundamental to your app’s operation. UIKit handles most window-related interactions, working with other objects as needed to implement many app behaviors.

You use windows only when you need to do the following:

- Provide a main window to display your app’s content.

- Create additional windows (as needed) to display additional content.

Normally, Xcode provides your app’s main window. New iOS projects use storyboards to define the app’s views. Storyboards require the presence of a window property on the app delegate object, which the Xcode templates automatically provide. If your app doesn’t use storyboards, you must create this window yourself.

Most apps need only one window, which displays the app’s content on the device’s main screen. Although you can create additional windows on the device’s main screen, extra windows are commonly used to display content on an external screen, as described in Presenting content on a connected display.

You also use UIWindow objects for a handful of other tasks:

- Setting the z-axis level of your window, which affects the visibility of the window relative to other windows.

- Showing windows and making them the target of keyboard events.

- Converting coordinate values to and from the window’s coordinate system.

- Changing the root view controller of a window.

- Changing the screen on which the window is displayed.

Windows don’t have any visual appearance of their own. Instead, a window hosts one or more views, which are managed by the window’s root view controller. You configure the root view controller in your storyboards, adding whatever views are appropriate for your interface.

You should rarely need to subclass UIWindow. The kinds of behaviors you might implement in a window can usually be implemented in a higher-level view controller more easily. One of the few times you might want to subclass is to override the becomeKey() or resignKey() methods to implement custom behaviors when a window’s key status changes. For information about how to display a window on a specific screen, see UIScreen.

### Understand keyboard interactions

Whereas touch events are delivered to the window where they occurred, events that don’t have a relevant coordinate value are delivered to the *key window*. Only one window at a time can be the key window, and you can use a window’s isKeyWindow property to determine its status. Most of the time, your app’s main window is the key window, but UIKit may designate a different window as needed.

If you need to know which window is key, observe the didBecomeKeyNotification and didResignKeyNotification notifications. The system sends those notifications on the main actor in response to key window changes in your app. To force a window become key, or to force a window to resign the key status, call the appropriate methods of this class.

## Topics

### Creating a window

init(windowScene: UIWindowScene)

Creates a window and associates it with the specified scene object.

### Configuring the window

var rootViewController: UIViewController?

The root view controller for the window.

var windowLevel: UIWindow.Level

The position of the window in the z-axis.

struct Level

The positioning of windows relative to each other.

var canResizeToFitContent: Bool

A Boolean value that indicates whether the window’s constraint-based content determines its size.

var screen: UIScreen

The screen to display the window on.

Deprecated

### Making windows key

var isKeyWindow: Bool

A Boolean value that indicates whether the window is the key window.

var canBecomeKey: Bool

A Boolean value that indicates whether the window can become the key window.

func makeKeyAndVisible()

Shows the window and makes it the key window.

func makeKey()

Makes the window the key window.

func becomeKey()

Tells the window that it’s the key window.

func resignKey()

Tells the window that it’s no longer the key window.

### Getting related objects

var windowScene: UIWindowScene?

The scene containing the window.

var avDisplayManager: AVDisplayManager

The display manager that handles requests for screen resolution, refresh rate, and HDR mode information.

### Converting coordinates

func convert(CGPoint, to: UIWindow?) -> CGPoint

Converts a point from the current window’s coordinate system to the coordinate system of another window.

func convert(CGPoint, from: UIWindow?) -> CGPoint

Converts a point from the coordinate system of a given window to the coordinate system of the current window.

func convert(CGRect, to: UIWindow?) -> CGRect

Converts a rectangle from the current window’s coordinate system to the coordinate system of another window.

func convert(CGRect, from: UIWindow?) -> CGRect

Converts a rectangle from the coordinate system of another window to coordinate system of the current window.

### Sending events

func sendEvent(UIEvent)

Dispatches the specified event to its views.

### Responding to window-related notifications

class let didBecomeVisibleNotification: NSNotification.Name

A notification that posts when a window becomes visible.

class let didBecomeHiddenNotification: NSNotification.Name

A notification that posts when a window becomes hidden.

class let didBecomeKeyNotification: NSNotification.Name

A notification that posts whenever a window becomes the key window.

class let didResignKeyNotification: NSNotification.Name

A notification that posts whenever a window resigns its status as main window.

### Responding to keyboard notifications

class let keyboardWillShowNotification: NSNotification.Name

A notification that posts immediately prior to displaying the keyboard.

class let keyboardDidShowNotification: NSNotification.Name

A notification that posts immediately after displaying the keyboard.

class let keyboardWillHideNotification: NSNotification.Name

A notification that posts immediately prior to dismissing the keyboard.

class let keyboardDidHideNotification: NSNotification.Name

A notification that posts immediately after dismissing the keyboard.

class let keyboardWillChangeFrameNotification: NSNotification.Name

A notification that posts immediately prior to a change in the keyboard’s frame.

class let keyboardDidChangeFrameNotification: NSNotification.Name

A notification that posts immediately after a change in the keyboard’s frame.

class let keyboardAnimationCurveUserInfoKey: String

A user info key to retrieve the animation curve that the system uses to animate the keyboard onto or off the screen.

class let keyboardAnimationDurationUserInfoKey: String

A user info key to retrieve the duration of the keyboard animation in seconds.

class let keyboardIsLocalUserInfoKey: String

A user info key to retrieve a Boolean value that indicates whether the keyboard belongs to the current app.

class let keyboardFrameBeginUserInfoKey: String

A user info key to retrieve the keyboard’s frame at the beginning of its animation.

class let keyboardFrameEndUserInfoKey: String

A user info key to retrieve the keyboard’s frame at the end of its animation.

### Working with layout guides

var safeAreaAspectFitLayoutGuide: any UILayoutGuide &amp; UILayoutGuideAspectFitting

A layout guide for placing content of a particular aspect ratio.

protocol UILayoutGuideAspectFitting

The interface for a layout guide that supports a particular aspect ratio.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Windows

protocol UICoordinateSpace

A set of methods for converting between different frames of reference on a screen.

