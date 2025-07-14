

- UIKit
-  UIViewController 

Class

# UIViewController

An object that manages a view hierarchy for your UIKit app.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIViewController
```

## Mentioned in 

Using responders and the responder chain to handle events

Displaying and managing views with a view controller

Creating a custom container view controller

Responding to memory warnings

## Overview

The UIViewController class defines the shared behavior that’s common to all view controllers. You rarely create instances of the UIViewController class directly. Instead, you subclass UIViewController and add the methods and properties needed to manage the view controller’s view hierarchy.

A view controller’s main responsibilities include the following:

- Updating the contents of the views, usually in response to changes to the underlying data

- Responding to user interactions with views

- Resizing views and managing the layout of the overall interface

- Coordinating with other objects — including other view controllers — in your app

A view controller is tightly bound to the views it manages and takes part in handling events in its view hierarchy. Specifically, view controllers are UIResponder objects and are inserted into the responder chain between the view controller’s root view and that view’s superview, which typically belongs to a different view controller. If none of the view controller’s views handle an event, the view controller has the option of handling the event or passing it along to the superview.

View controllers are rarely used in isolation. Instead, you often use multiple view controllers, each of which owns a portion of your app’s user interface. For example, one view controller might display a table of items while a different view controller displays the selected item from that table. Usually, only the views from one view controller are visible at a time. A view controller may present a different view controller to display a new set of views, or it may act as a container for other view controllers’ content and animate views however it wants.

### Subclassing notes

Every app contains at least one custom subclass of UIViewController. More often, apps contain many custom view controllers. Custom view controllers define the overall behaviors of your app, including the app’s appearance and how it responds to user interactions. The following sections provide a brief overview of some of the tasks your custom subclass performs. For detailed information about using and implementing view controllers, see View Controller Programming Guide for iOS.

#### Manage views

Each view controller manages a view hierarchy, the root view of which is stored in the view property of this class. The root view acts primarily as a container for the rest of the view hierarchy. The size and position of the root view is determined by the object that owns it, which is either a parent view controller or the app’s window. The view controller that’s owned by the window is the app’s root view controller and its view is sized to fill the window.

View controllers load their views lazily. Accessing the view property for the first time loads or creates the view controller’s views. There are several ways to specify the views for a view controller:

- Specify the view controller and its views in your app’s storyboard. Storyboards are the preferred way to specify your views. With a storyboard, you specify the views and their connections to the view controller. You also specify the relationships and segues between your view controllers, which makes it easier to see and modify your app’s behavior.

To load a view controller from a storyboard, call the instantiateViewController(withIdentifier:) method of the appropriate UIStoryboard object. The storyboard object creates the view controller and returns it to your code.

- Specify the views for a view controller using a nib file. A nib file lets you specify the views of a single view controller but doesn’t let you define segues or relationships between view controllers. The nib file also stores only minimal information about the view controller itself.

To initialize a view controller object using a nib file, create your view controller class programmatically and initialize it using the init(nibName:bundle:) method. When its views are requested, the view controller loads them from the nib file.

- Specify the views for a view controller using the loadView() method. In that method, create your view hierarchy programmatically and assign the root view of that hierarchy to the view controller’s view property.

All of these techniques have the same end result, which is to create the appropriate set of views and expose them through the view property.

Important

A view controller is the sole owner of its view and any subviews it creates. It’s responsible for creating those views and for relinquishing ownership of them at the appropriate times such as when the view controller itself is released. If you use a storyboard or a nib file to store your view objects, each view controller object automatically gets its own copy of these views when the view controller asks for them. However, if you create your views manually, each view controller must have its own unique set of views. You can’t share views between view controllers.

A view controller’s root view is always sized to fit its assigned space. For other views in your view hierarchy, use Interface Builder to specify the Auto Layout constraints that govern how each view is positioned and sized within its superview’s bounds. You can also create constraints programmatically and add them to your views at appropriate times. For more information about how to create constraints, see Auto Layout Guide.

##### Handle view-related notifications

When the visibility of its views changes, a view controller automatically calls its own methods so that subclasses can respond to the change. Use a method like viewIsAppearing(_:) to prepare your views to appear onscreen, and use viewWillDisappear(_:) to save changes or other state information. Use other methods to make appropriate changes.

The following image shows the possible visible states for a view controller’s views and the state transitions that can occur. Not all `will` callback methods are paired with only a `did` callback method. You need to ensure that if you start a process in a `will` callback method, you end the process in both the corresponding `did` and the opposite `will` callback method.

##### Handle view rotations

As of iOS 8, all rotation-related methods are deprecated. Instead, rotations are treated as a change in the size of the view controller’s view and are therefore reported using the viewWillTransition(to:with:) method. When the interface orientation changes, UIKit calls this method on the window’s root view controller. That view controller then notifies its child view controllers, propagating the message throughout the view controller hierarchy.

In iOS 6 and iOS 7, your app supports the interface orientations defined in your app’s `Info.plist` file. A view controller can override the supportedInterfaceOrientations method to limit the list of supported orientations. Typically, the system calls this method only on the root view controller of the window or a view controller presented to fill the entire screen; child view controllers use the portion of the window provided for them by their parent view controller and no longer participate directly in decisions about what rotations are supported. The intersection of the app’s orientation mask and the view controller’s orientation mask is used to determine which orientations a view controller can be rotated into.

You can override the preferredInterfaceOrientationForPresentation for a view controller that’s intended to be presented full screen in a specific orientation.

When a rotation occurs for a visible view controller, the willRotate(to:duration:), willAnimateRotation(to:duration:), and didRotate(from:) methods are called during the rotation. The viewWillLayoutSubviews() method is also called after the view is resized and positioned by its parent. If a view controller isn’t visible when an orientation change occurs, then the rotation methods are never called. However, the viewWillLayoutSubviews() method is called when the view becomes visible.

Note

At launch time, apps should always set up their interface in a portrait orientation. After the application(_:didFinishLaunchingWithOptions:) method returns, the app uses the view controller rotation mechanism described above to rotate the views to the appropriate orientation prior to showing the window.

#### Implement a container view controller

A custom UIViewController subclass can also act as a container view controller. A container view controller manages the presentation of content of other view controllers it owns, also known as its child view controllers. A child’s view can be presented as-is or in conjunction with views owned by the container view controller.

Your container view controller subclass should declare a public interface to associate its children. The nature of these methods is up to you and depends on the semantics of the container you’re creating. You need to decide how many children can be displayed by your view controller at once, when those children are displayed, and where they appear in your view controller’s view hierarchy. Your view controller class defines what relationships, if any, are shared by the children. By establishing a clean public interface for your container, you ensure that children use its capabilities logically, without accessing too many private details about how your container implements the behavior.

Your container view controller must associate a child view controller with itself before adding the child’s root view to the view hierarchy. This allows iOS to properly route events to child view controllers and the views those controllers manage. Likewise, after it removes a child’s root view from its view hierarchy, it should disconnect that child view controller from itself. To make or break these associations, your container calls specific methods defined by the base class. These methods aren’t intended to be called by clients of your container class; they are to be used only by your container’s implementation to provide the expected containment behavior.

Here are the essential methods you might need to call:

- addChild(_:)

- removeFromParent()

- willMove(toParent:)

- didMove(toParent:)

Note

You’re not required to override any methods when creating a container view controller.

By default, rotation and appearance callbacks are automatically forwarded to children. You may optionally override the shouldAutomaticallyForwardRotationMethods() and shouldAutomaticallyForwardAppearanceMethods methods to take control of this behavior yourself.

#### Manage memory

Memory is a critical resource in iOS, and view controllers provide built-in support for reducing their memory footprint at critical times. The UIViewController class provides some automatic handling of low-memory conditions through its didReceiveMemoryWarning() method, which releases unneeded memory.

#### Support state preservation and restoration

If you assign a value to the view controller’s restorationIdentifier property, the system may ask the view controller to encode itself when the app transitions to the background. When preserved, a view controller preserves the state of any views in its view hierarchy that also have restoration identifiers. View controllers don’t automatically save any other state. If you’re implementing a custom container view controller, you must encode any child view controllers yourself. Each child you encode must have a unique restoration identifier.

For more information about how the system determines which view controllers to preserve and restore, see App Programming Guide for iOS. To see an example of state preservation and restoration, see Restoring your app’s state.

## Topics

### Creating a view controller

init(nibName: String?, bundle: Bundle?)

Creates a view controller with the nib file in the specified bundle.

init?(coder: NSCoder)

Creates a view controller with data in an unarchiver.

### Getting the storyboard and nib information

var storyboard: UIStoryboard?

The storyboard from which the view controller originated.

var nibName: String?

The name of the view controller’s nib file, if one was specified.

var nibBundle: Bundle?

The view controller’s nib bundle if it exists.

### Managing the view

var view: UIView!

The view that the controller manages.

var viewIfLoaded: UIView?

The view controller’s view, or `nil` if the view isn’t yet loaded.

var isViewLoaded: Bool

A Boolean value indicating whether the view is currently loaded into memory.

func loadView()

Creates the view that the controller manages.

func viewDidLoad()

Called after the controller’s view is loaded into memory.

func loadViewIfNeeded()

Loads the view controller’s view if it’s not loaded yet.

var title: String?

A localized string that represents the view this controller manages.

var preferredContentSize: CGSize

The preferred size for the view controller’s view.

### Responding to view-related events

func viewWillAppear(Bool)

Notifies the view controller that its view is about to be added to a view hierarchy.

func viewIsAppearing(Bool)

Notifies the view controller that the system is adding the view controller’s view to a view hierarchy.

func viewDidAppear(Bool)

Notifies the view controller that its view was added to a view hierarchy.

func viewWillDisappear(Bool)

Notifies the view controller that its view is about to be removed from a view hierarchy.

func viewDidDisappear(Bool)

Notifies the view controller that its view was removed from a view hierarchy.

var isBeingDismissed: Bool

A Boolean value indicating whether the view controller is in the process of being dismissed by one of its ancestors.

var isBeingPresented: Bool

A Boolean value indicating whether the view controller in the process of being presented by one of its ancestors.

var isMovingFromParent: Bool

A Boolean value indicating whether the view controller is moving from a parent view controller.

var isMovingToParent: Bool

A Boolean value indicating whether the view controller is moving to a parent view controller.

### Extending the view’s safe area

Positioning content relative to the safe area

Position views so that they aren’t obstructed by other content.

var additionalSafeAreaInsets: UIEdgeInsets

Custom insets that you specify to modify the view controller’s safe area.

func viewSafeAreaInsetsDidChange()

Called to notify the view controller that the safe area insets of its root view changed.

### Managing the view’s margins

Positioning content within layout margins

Position views so that they aren’t crowded by other content.

var viewRespectsSystemMinimumLayoutMargins: Bool

A Boolean value indicating whether the view controller’s view uses the system-defined minimum layout margins.

var systemMinimumLayoutMargins: NSDirectionalEdgeInsets

The minimum layout margins for the view controller’s root view.

func viewLayoutMarginsDidChange()

Called to notify the view controller that the layout margins of its root view changed.

### Configuring the view’s layout behavior

var edgesForExtendedLayout: UIRectEdge

The edges that you extend for your view controller.

struct UIRectEdge

Constants that specify the edges of a rectangle.

var extendedLayoutIncludesOpaqueBars: Bool

A Boolean value indicating whether or not the extended layout includes opaque bars.

func viewWillLayoutSubviews()

Notifies the view controller that its view is about to lay out its subviews.

func viewDidLayoutSubviews()

Notifies the view controller when its view finishes laying out its subviews.

func updateViewConstraints()

Notifies the view controller when its view needs to update its constraints.

### Configuring the view rotation settings

var supportedInterfaceOrientations: UIInterfaceOrientationMask

The interface orientations that the view controller supports.

var preferredInterfaceOrientationForPresentation: UIInterfaceOrientation

The interface orientation to use when presenting the view controller.

func setNeedsUpdateOfSupportedInterfaceOrientations()

Notifies the view controller about a change in supported interface orientations or preferred interface orientation for presentation.

### Performing segues

func shouldPerformSegue(withIdentifier: String, sender: Any?) -> Bool

Determines whether the segue with the specified identifier should be performed.

func prepare(for: UIStoryboardSegue, sender: Any?)

Notifies the view controller that a segue is about to be performed.

func performSegue(withIdentifier: String, sender: Any?)

Initiates the segue with the specified identifier from the current view controller’s storyboard file.

func allowedChildrenForUnwinding(from: UIStoryboardUnwindSegueSource) -> [UIViewController]

Returns an array of child view controllers to search for an unwind segue destination.

func childContaining(UIStoryboardUnwindSegueSource) -> UIViewController?

Returns the child view controller that contains the source of the unwind segue.

func canPerformUnwindSegueAction(Selector, from: UIViewController, sender: Any?) -> Bool

Called on a view controller to determine whether it responds to an unwind action.

func unwind(for: UIStoryboardSegue, towards: UIViewController)

Called when an unwind segue transitions to a new view controller.

### Presenting a view controller

func show(UIViewController, sender: Any?)

Presents a view controller in a primary context.

func showDetailViewController(UIViewController, sender: Any?)

Presents a view controller in a secondary (or detail) context.

func present(UIViewController, animated: Bool, completion: (() -> Void)?)

Presents a view controller modally.

func dismiss(animated: Bool, completion: (() -> Void)?)

Dismisses the view controller that was presented modally by the view controller.

var modalPresentationStyle: UIModalPresentationStyle

The presentation style for modal view controllers.

enum UIModalPresentationStyle

Modal presentation styles available when presenting view controllers.

var modalTransitionStyle: UIModalTransitionStyle

The transition style to use when presenting the view controller.

enum UIModalTransitionStyle

Transition styles available when presenting view controllers.

var isModalInPresentation: Bool

A Boolean value indicating whether the view controller enforces a modal behavior.

var definesPresentationContext: Bool

A Boolean value that indicates whether this view controller’s view is covered when the view controller or one of its descendants presents a view controller.

var providesPresentationContextTransitionStyle: Bool

A Boolean value that indicates whether the view controller specifies the transition style for view controllers it presents.

var disablesAutomaticKeyboardDismissal: Bool

Returns a Boolean indicating whether the current input view is dismissed automatically when changing controls.

class let showDetailTargetDidChangeNotification: NSNotification.Name

Posted when a split view controller is expanded or collapsed.

### Adding a custom transition or presentation

var transitioningDelegate: (any UIViewControllerTransitioningDelegate)?

The delegate object that provides transition animator, interactive controller, and custom presentation controller objects.

var transitionCoordinator: (any UIViewControllerTransitionCoordinator)?

Returns the active transition coordinator object.

func targetViewController(forAction: Selector, sender: Any?) -> UIViewController?

Returns the view controller that responds to the action.

var presentationController: UIPresentationController?

The presentation controller that’s managing the current view controller.

var popoverPresentationController: UIPopoverPresentationController?

The nearest popover presentation controller that is managing the current view controller.

var sheetPresentationController: UISheetPresentationController?

The sheet presentation controller for the view controller.

var activePresentationController: UIPresentationController?

The presentation controller that’s managing the view controller.

var restoresFocusAfterTransition: Bool

A Boolean value that indicates whether an item that previously was focused should again become focused when the item’s view controller becomes visible and focusable.

Customizing and resizing sheets in UIKit

Discover how to create a layered and customized sheet experience in UIKit.

### Adapting to environment changes

func collapseSecondaryViewController(UIViewController, for: UISplitViewController)

Called when a split view controller transitions to a compact-width size class.

func separateSecondaryViewController(for: UISplitViewController) -> UIViewController?

Called when a split view controller transitions to a regular-width size class.

### Adjusting the interface style

var overrideUserInterfaceStyle: UIUserInterfaceStyle

The user interface style adopted by the view controller and all of its children.

var preferredUserInterfaceStyle: UIUserInterfaceStyle

The preferred interface style for this view controller.

var childViewControllerForUserInterfaceStyle: UIViewController?

The child view controller that supports the preferred user interface style.

func setNeedsUserInterfaceAppearanceUpdate()

Notifies the view controller that a change occurred that might affect the preferred interface style.

enum UIUserInterfaceStyle

Constants that indicate the interface style for the app.

### Observing trait changes

protocol UITraitChangeObservable

A type that calls your code in reaction to changes in the trait environment.

### Overriding trait values

var traitOverrides: UITraitOverrides

struct UITraitOverrides

### Managing child view controllers in a custom container

var children: [UIViewController]

An array of view controllers that are children of the current view controller.

func addChild(UIViewController)

Adds the specified view controller as a child of the current view controller.

func removeFromParent()

Removes the view controller from its parent.

func transition(from: UIViewController, to: UIViewController, duration: TimeInterval, options: UIView.AnimationOptions, animations: (() -> Void)?, completion: ((Bool) -> Void)?)

Transitions between two of the view controller’s child view controllers.

var shouldAutomaticallyForwardAppearanceMethods: Bool

Returns a Boolean value indicating whether appearance methods are forwarded to child view controllers.

func beginAppearanceTransition(Bool, animated: Bool)

Tells a child controller its appearance is about to change.

func endAppearanceTransition()

Tells a child controller its appearance has changed.

class let hierarchyInconsistencyException: NSExceptionName

Raised if the view controller hierarchy is inconsistent with the view hierarchy.

### Responding to containment events

func willMove(toParent: UIViewController?)

Called just before the view controller is added or removed from a container view controller.

func didMove(toParent: UIViewController?)

Called after the view controller is added or removed from a container view controller.

### Getting other related view controllers

var presentingViewController: UIViewController?

The view controller that presented this view controller.

var presentedViewController: UIViewController?

The view controller that is presented by this view controller, or one of its ancestors in the view controller hierarchy.

var parent: UIViewController?

The parent view controller of the recipient.

var splitViewController: UISplitViewController?

The nearest ancestor in the view controller hierarchy that is a split view controller.

var navigationController: UINavigationController?

The nearest ancestor in the view controller hierarchy that is a navigation controller.

var tabBarController: UITabBarController?

The nearest ancestor in the view controller hierarchy that is a tab bar controller.

### Configuring a navigation interface

var navigationItem: UINavigationItem

The navigation item used to represent the view controller in a parent’s navigation bar.

var hidesBottomBarWhenPushed: Bool

A Boolean value indicating whether the toolbar at the bottom of the screen is hidden when the view controller is pushed on to a navigation controller.

func setToolbarItems([UIBarButtonItem]?, animated: Bool)

Sets the toolbar items to be displayed along with the view controller.

var toolbarItems: [UIBarButtonItem]?

The toolbar items associated with the view controller.

### Configuring tab bar content

var tabBarItem: UITabBarItem!

The tab bar item that represents the view controller when added to a tab bar controller.

var tabBarObservedScrollView: UIScrollView?

The full-screen scroll view to synchronize with a scrolling tab bar.

Deprecated

### Working with scrolling content

func setContentScrollView(UIScrollView?, for: NSDirectionalRectEdge)

Sets the scroll view that bars observe for the specified edge.

func setContentScrollView(UIScrollView?)

Sets the scroll view that bars observe for all edges of the view.

func contentScrollView(for: NSDirectionalRectEdge) -> UIScrollView?

Returns the scroll view the view controller observes for the specified edge.

### Indicating missing content

var contentUnavailableConfiguration: (any UIContentConfiguration)?

The current content-unavailable configuration of the view controller.

var contentUnavailableConfigurationState: UIContentUnavailableConfigurationState

The current configuration state of the content-unavailable view.

func setNeedsUpdateContentUnavailableConfiguration()

Requests that the system update the content-unavailable configuration for the latest state.

func updateContentUnavailableConfiguration(using: UIContentUnavailableConfigurationState)

Updates the content-unavailable configuration for the provided state.

struct UIContentUnavailableConfiguration

A content configuration for a content-unavailable view.

### Supporting app extensions

var extensionContext: NSExtensionContext?

Returns the extension context of the view controller.

### Coordinating with system gestures

var preferredScreenEdgesDeferringSystemGestures: UIRectEdge

The screen edges for which you want your gestures to take precedence over the system gestures.

var childForScreenEdgesDeferringSystemGestures: UIViewController?

Returns the child view controller that should be queried to see if its gestures should take precedence.

func setNeedsUpdateOfScreenEdgesDeferringSystemGestures()

Notifies the system of changes to the screen edges that defer system gestures.

var prefersHomeIndicatorAutoHidden: Bool

A Boolean that indicates whether the system is allowed to hide the visual indicator for returning to the Home Screen.

var childForHomeIndicatorAutoHidden: UIViewController?

Returns the child view controller that is consulted about its preference for displaying a visual indicator for returning to the Home screen.

func setNeedsUpdateOfHomeIndicatorAutoHidden()

Notifies UIKit that your view controller updated its preference regarding the visual indicator for returning to the Home screen.

### Working with transitions

var preferredTransition: UIViewController.Transition?

An object that defines the transition animation when switching to the view controller.

class Transition

An object that defines the transition animation when switching to a new view controller.

### Working with focus

var focusGroupIdentifier: String?

The identifier of the focus group that the view controller belongs to.

### Managing pointer lock state

var prefersPointerLocked: Bool

A Boolean value that indicates whether the view controller prefers to lock the pointer to a specific scene.

func setNeedsUpdateOfPrefersPointerLocked()

Indicates that the view controller changed the pointer lock preference.

var childViewControllerForPointerLock: UIViewController?

A child view controller to query for the pointer lock preference.

### Managing the status bar

var prefersStatusBarHidden: Bool

Specifies whether the view controller prefers the status bar to be hidden or shown.

var childForStatusBarHidden: UIViewController?

The view controller to use for determining the hidden state of the status bar.

var childForStatusBarStyle: UIViewController?

Called when the system needs the view controller to use for determining status bar style.

var preferredStatusBarStyle: UIStatusBarStyle

The preferred status bar style for the view controller.

enum UIStatusBarStyle

Constants that describe the style of the device’s status bar.

var modalPresentationCapturesStatusBarAppearance: Bool

Specifies whether a view controller, presented non-fullscreen, takes over control of status bar appearance from the presenting view controller.

var preferredStatusBarUpdateAnimation: UIStatusBarAnimation

Specifies the animation style to use for hiding and showing the status bar for the view controller.

func setNeedsStatusBarAppearanceUpdate()

Indicates to the system that the view controller status bar attributes have changed.

### Managing the Touch Bar

var childViewControllerForTouchBar: UIViewController?

The child view controller that the system uses to display content in the Touch Bar.

func setNeedsTouchBarUpdate()

Tells the system to update the Touch Bar.

### Accessing the available key commands

var performsActionsWhilePresentingModally: Bool

A Boolean value indicating whether the view controller performs menu-related actions.

func addKeyCommand(UIKeyCommand)

Associates the specified keyboard shortcut with the view controller.

func removeKeyCommand(UIKeyCommand)

Removes the key command from the view controller.

### Adding editing behaviors to your view controller

var isEditing: Bool

A Boolean value indicating whether the view controller currently allows the user to edit the view contents.

func setEditing(Bool, animated: Bool)

Sets whether the view controller shows an editable view.

var editButtonItem: UIBarButtonItem

Returns a bar button item that toggles its title and associated state between Edit and Done.

### Handling memory warnings

func didReceiveMemoryWarning()

Sent to the view controller when the app receives a memory warning.

### Managing state restoration

Restoring your app’s state

Provide continuity for the user by preserving current activities.

var restorationIdentifier: String?

The identifier that determines whether the view controller supports state restoration.

var restorationClass: (any UIViewControllerRestoration.Type)?

The class responsible for recreating this view controller when restoring the app’s state.

func encodeRestorableState(with: NSCoder)

Encodes state-related information for the view controller.

func decodeRestorableState(with: NSCoder)

Decodes and restores state-related information for the view controller.

func applicationFinishedRestoringState()

Called on restored view controllers after other object decoding is complete.

### Logging user interaction intervals

var interactionActivityTrackingBaseName: String?

The base name the view controller uses for logging signposts that annotate user interactions.

### Supporting types

struct ViewLoading

A property wrapper that loads the view controller’s view before accessing the property.

enum UIContainerBackgroundStyle

### Deprecated

Deprecated symbols

Symbols that view controllers no longer support.

### Instance Properties

var childViewControllerForPreferredContainerBackgroundStyle: UIViewController?

var ornaments: [UIOrnament]

var preferredContainerBackgroundStyle: UIContainerBackgroundStyle

var tab: UITab?

### Instance Methods

func setNeedsUpdateOfPreferredContainerBackgroundStyle()

func updateTraitsIfNeeded()

## Relationships

### Inherits From

- UIResponder

### Inherited By

- UIActivityViewController
- UIAlertController
- UICloudSharingController
- UICollectionViewController
- UIColorPickerViewController
- UIDocumentBrowserViewController
- UIDocumentMenuViewController
- UIDocumentPickerExtensionViewController
- UIDocumentPickerViewController
- UIDocumentViewController
- UIFontPickerViewController
- UIInputViewController
- UINavigationController
- UIPageViewController
- UIReferenceLibraryViewController
- UISearchContainerViewController
- UISearchController
- UISplitViewController
- UITabBarController
- UITableViewController
- UITextFormattingViewController

### Conforms To

- CVarArg
- Copyable
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

### Content view controllers

Displaying and managing views with a view controller

Build a view controller in storyboards, configure it with custom views, and fill those views with your app’s data.

Showing and hiding view controllers

Display view controllers using different techniques, and pass data between them during transitions.

class UITableViewController

A view controller that specializes in managing a table view.

class UICollectionViewController

A view controller that specializes in managing a collection view.

protocol UIContentContainer

A set of methods for adapting the contents of your view controllers to size and trait changes.

