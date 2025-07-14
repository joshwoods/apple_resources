

- UIKit
-  UIApplication 

Class

# UIApplication

The centralized point of control and coordination for apps running in iOS.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIApplication
```

## Mentioned in 

Using responders and the responder chain to handle events

About the UI preservation process

About App Development with UIKit

Handling key presses made on a physical keyboard

About the app launch sequence

## Overview

Every iOS app has exactly one instance of UIApplication (or, very rarely, a subclass of UIApplication). When an app launches, the system calls the UIApplicationMain(_:_:_:_:) function. Among its other tasks, this function creates a singleton UIApplication object that you access using shared.

Your app’s application object handles the initial routing of incoming user events. It dispatches action messages forwarded to it by control objects (instances of the UIControl class) to appropriate target objects. The application object maintains a list of open windows (UIWindow objects), which it can use to retrieve any of the app’s UIView objects.

The UIApplication class defines a delegate that conforms to the UIApplicationDelegate protocol and must implement some of the protocol’s methods. The application object informs the delegate of significant runtime events—for example, app launch, low-memory warnings, and app termination—giving it an opportunity to respond appropriately.

Apps can cooperatively handle a resource, such as an email or an image file, through the open(_:options:completionHandler:) method. For example, an app that calls this method with an email URL causes the Mail app to launch and display the message.

The APIs in this class allow you to manage device-specific behavior. Use your UIApplication object to do the following:

- Temporarily suspend incoming touch events (beginIgnoringInteractionEvents())

- Register for remote notifications (registerForRemoteNotifications())

- Trigger the undo-redo UI (applicationSupportsShakeToEdit)

- Determine whether there is an installed app registered to handle a URL scheme (canOpenURL(_:))

- Extend the execution of the app so that it can finish a task in the background (beginBackgroundTask(expirationHandler:) and beginBackgroundTask(withName:expirationHandler:))

- Schedule and cancel local notifications (scheduleLocalNotification(_:) and cancelLocalNotification(_:))

- Coordinate the reception of remote-control events (beginReceivingRemoteControlEvents() and endReceivingRemoteControlEvents())

- Perform app-level state restoration tasks (methods in the Managing state restoration task group)

### Subclassing notes

Most apps don’t need to subclass UIApplication. Instead, use an app delegate to manage interactions between the system and the app.

If your app must handle incoming events before the system does—a very rare situation—you can implement a custom event or action dispatching mechanism. To do this, subclass UIApplication and override the sendEvent(_:) and/or the sendAction(_:to:from:for:) methods. For every event you intercept, after you handle the event, dispatch it back to the system by calling:

```
super.sendEvent(event)
```

Intercepting events is only rarely required and you should avoid it if possible.

## Topics

### Accessing the shared application

class var shared: UIApplication

The singleton app instance.

### Configuring your app’s behavior

var delegate: (any UIApplicationDelegate)?

The delegate of the app object.

protocol UIApplicationDelegate

A set of methods to manage shared behaviors for your app.

### Registering for remote notifications

func registerForRemoteNotifications()

Registers to receive remote notifications through Apple Push Notification service.

func unregisterForRemoteNotifications()

Unregisters for all remote notifications received through Apple Push Notification service.

var isRegisteredForRemoteNotifications: Bool

A Boolean value that indicates whether the app is currently registered for remote notifications.

### Getting the application state

var applicationState: UIApplication.State

The app’s current state, or that of its most active scene.

enum State

Constants that indicate the running states of an app.

### Getting scene information

var supportsMultipleScenes: Bool

A Boolean value that indicates whether the app may display multiple scenes simultaneously.

var connectedScenes: Set&lt;UIScene>

The app’s currently connected scenes.

var openSessions: Set&lt;UISceneSession>

The sessions whose scenes are either currently active or archived by the system.

### Managing a scene’s life cycle

func activateSceneSession(for: UISceneSessionActivationRequest, errorHandler: ((any Error) -> Void)?)

Asks the system to activate an existing scene or create a new scene and associate it with your app.

func requestSceneSessionDestruction(UISceneSession, options: UISceneDestructionRequestOptions?, errorHandler: ((any Error) -> Void)?)

Asks the system to dismiss an existing scene and remove it from the app switcher.

func requestSceneSessionRefresh(UISceneSession)

Asks the system to update any system UI associated with the specified scene.

struct UISceneSessionActivationRequest

A collection of properties that you use to request activation of a scene.

class ActivationRequestOptions

An object that contains information you want the system to use when activating the session associated with a scene.

class UISceneDestructionRequestOptions

An object you pass to UIKit to permanently remove a scene and its associated session from your app.

### Managing background tasks

var backgroundRefreshStatus: UIBackgroundRefreshStatus

Indicates whether the app can refresh content when running in the background.

enum UIBackgroundRefreshStatus

Constants that indicate whether background execution is enabled for the app.

class let backgroundRefreshStatusDidChangeNotification: NSNotification.Name

A notification that posts when the app’s status for downloading content in the background changes.

func beginBackgroundTask(withName: String?, expirationHandler: (() -> Void)?) -> UIBackgroundTaskIdentifier

Marks the start of a task with a custom name that should continue if the app enters the background.

func beginBackgroundTask(expirationHandler: (() -> Void)?) -> UIBackgroundTaskIdentifier

Marks the start of a task that should continue if the app enters the background.

func endBackgroundTask(UIBackgroundTaskIdentifier)

Marks the end of a specific long-running background task.

struct UIBackgroundTaskIdentifier

A unique token that identifies a request to run in the background.

var backgroundTimeRemaining: TimeInterval

The maximum amount of time remaining for the app to run in the background.

### Fetching content in the background

class let backgroundFetchIntervalMinimum: TimeInterval

The smallest fetch interval supported by the system.

class let backgroundFetchIntervalNever: TimeInterval

A fetch interval large enough to prevent fetch operations from occurring.

### Opening a URL resource

func open(URL, options: [UIApplication.OpenExternalURLOptionsKey : Any], completionHandler: ((Bool) -> Void)?)

Attempts to asynchronously open the resource at the specified URL.

func canOpenURL(URL) -> Bool

Returns a Boolean value that indicates whether an app is available to handle a URL scheme.

struct OpenExternalURLOptionsKey

Options for opening a URL.

### Deep linking to custom settings

class let openSettingsURLString: String

The URL string you use to deep link to your app’s custom settings in the Settings app.

static let openNotificationSettingsURLString: String

The URL string you use to deep link to your app’s notification settings in the Settings app.

let UIApplicationOpenNotificationSettingsURLString: String

A constant that provides the URL string you use to deep link to your app’s notification settings in the Settings app.

Deprecated

class let openDefaultApplicationsSettingsURLString: String

The URL string used to select a default app in the Settings app.

### Managing the app’s idle timer

var isIdleTimerDisabled: Bool

A Boolean value that controls whether the idle timer is disabled for the app.

### Managing state restoration

func extendStateRestoration()

Tells the app that your code is restoring state asynchronously.

func completeStateRestoration()

Tells the app that your code has finished any asynchronous state restoration.

func ignoreSnapshotOnNextApplicationLaunch()

Prevents the app from using the recent snapshot image during the next launch cycle.

class func registerObject(forStateRestoration: any UIStateRestoring, restorationIdentifier: String)

Registers a custom object for use with the state restoration system.

### Providing an app’s shortcut items

var shortcutItems: [UIApplicationShortcutItem]?

The Home screen dynamic quick actions for your app; available on devices that support 3D Touch.

### Accessing protected content

var isProtectedDataAvailable: Bool

A Boolean value that indicates whether content protection is active.

class let protectedDataDidBecomeAvailableNotification: NSNotification.Name

A notification that posts when the protected files become available for your code to access.

class let protectedDataWillBecomeUnavailableNotification: NSNotification.Name

A notification that posts shortly before protected files are locked down and become inaccessible.

### Receiving remote control events

func beginReceivingRemoteControlEvents()

Tells the app to begin receiving remote-control events.

func endReceivingRemoteControlEvents()

Tells the app to stop receiving remote-control events.

### Accessing the layout direction

var userInterfaceLayoutDirection: UIUserInterfaceLayoutDirection

The layout direction of the user interface.

enum UIUserInterfaceLayoutDirection

Constants that specify the directional flow of the user interface.

### Controlling and handling events

func sendEvent(UIEvent)

Dispatches an event to the appropriate responder objects in the app.

func sendAction(Selector, to: Any?, from: Any?, for: UIEvent?) -> Bool

Sends an action message identified by the selector to a specified target.

var applicationSupportsShakeToEdit: Bool

A Boolean value that determines whether shaking the device displays the undo-redo user interface.

### Managing the app’s icon

var supportsAlternateIcons: Bool

A Boolean value that indicates whether the app is allowed to change its icon.

var alternateIconName: String?

The name of the icon the system displays for the app.

func setAlternateIconName(String?, completionHandler: (((any Error)?) -> Void)?)

Changes the icon the system displays for the app.

### Managing the preferred content size

var preferredContentSizeCategory: UIContentSizeCategory

The font sizing option preferred by the user.

struct UIContentSizeCategory

Constants that indicate the preferred size of your content.

protocol UIContentSizeCategoryAdjusting

A collection of methods that give controls an easy way to adopt automatic adjustment to content category changes.

static let didChangeNotification: NSNotification.Name

A notification that posts when the user changes the preferred content size setting.

static let newValueUserInfoKey: String

A key that reflects the new preferred content size.

### Specifying the supported interface orientations

func supportedInterfaceOrientations(for: UIWindow?) -> UIInterfaceOrientationMask

Returns the default set of interface orientations to use for the view controllers in the specified window.

### Tracking controls in the run loop

static let tracking: RunLoop.Mode

The mode set while tracking in controls takes place.

### Detecting screenshots

class let userDidTakeScreenshotNotification: NSNotification.Name

A notification that posts when a person takes a screenshot on the device.

### Discovering if your app is the default app in a category

func isDefault(UIApplication.Category) throws -> Bool

Reports whether this app is the person’s default app in the given category.

enum Category

Constants that describe the types of apps in the system.

struct CategoryDefaultError

Errors that can happen when the system checks if your app is the default app in a category.

### Deprecated

Deprecated symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- UIResponder

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIUserActivityRestoring

## See Also

### Life cycle

Managing your app’s life cycle

Respond to system notifications when your app is in the foreground or background, and handle other significant system-related events.

Responding to the launch of your app

Initialize your app’s data structures, prepare your app to run, and respond to any launch-time requests from the system.

protocol UIApplicationDelegate

A set of methods to manage shared behaviors for your app.

Scenes

Manage multiple instances of your app’s UI simultaneously, and direct resources to the appropriate instance of your UI.

