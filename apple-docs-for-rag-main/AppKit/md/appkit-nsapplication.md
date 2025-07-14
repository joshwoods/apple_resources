

- AppKit
-  NSApplication 

Class

# NSApplication

An object that manages an app’s main event loop and resources used by all of that app’s objects.

macOS

``` source
@MainActor
class NSApplication
```

## Mentioned in 

Passing control from one app to another with cooperative activation

Choosing a Specific Appearance for Your macOS App

## Overview

Every app uses a single instance of NSApplication to control the main event loop, keep track of the app’s windows and menus, distribute events to the appropriate objects (that’s, itself or one of its windows), set up autorelease pools, and receive notification of app-level events. An NSApplication object has a delegate (an object that you assign) that’s notified when the app starts or terminates, is hidden or activated, should open a file selected by the user, and so forth. By setting the delegate and implementing the delegate methods, you customize the behavior of your app without having to subclass NSApplication. In your app’s `main()` function, create the NSApplication instance by calling the shared class method. After creating the application object, the `main()` function should load your app’s main nib file and then start the event loop by sending the application object a run() message. If you create an Application project in Xcode, this `main()` function is created for you. The `main()` function Xcode creates begins by calling a function named `NSApplicationMain()`, which is functionally similar to the following:

```
void NSApplicationMain(int argc, char *argv[]) {
    [NSApplication sharedApplication];
    [NSBundle loadNibNamed:@"myMain" owner:NSApp];
    [NSApp run];
}
```

The shared class method initializes the display environment and connects your program to the window server and the display server. The NSApplication object maintains a list of all the NSWindow objects the app uses, so it can retrieve any of the app’s NSView objects. The shared method also initializes the global variable `NSApp`, which you use to retrieve the NSApplication instance. shared only performs the initialization once. If you invoke it more than once, it returns the application object it created previously.

The shared NSApplication object performs the important task of receiving events from the window server and distributing them to the proper NSResponder objects. `NSApp` translates an event into an NSEvent object, then forwards the event object to the affected NSWindow object. All keyboard and mouse events go directly to the NSWindow object associated with the event. The only exception to this rule is if the Command key is pressed when a key-down event occurs; in this case, every NSWindow object has an opportunity to respond to the event. When a window object receives an NSEvent object from `NSApp`, it distributes it to the objects in its view hierarchy.

NSApplication is also responsible for dispatching certain Apple events received by the app. For example, macOS sends Apple events to your app at various times, such as when the app is launched or reopened. NSApplication installs Apple event handlers to handle these events by sending a message to the appropriate object. You can also use the NSAppleEventManager class to register your own Apple event handlers. The applicationWillFinishLaunching(_:) method is generally the best place to do so. For more information on how events are handled and how you can modify the default behavior, including information on working with Apple events in scriptable apps, see How Cocoa Applications Handle Apple Events in Cocoa Scripting Guide.

The NSApplication class sets up `@autorelease` block during initialization and inside the event loop—specifically, within its initialization (or shared) and run() methods. Similarly, the methods AppKit adds to Bundle employ `@autorelease` blocks during the loading of nib files. These `@autorelease` blocks aren’t accessible outside the scope of the respective NSApplication and Bundle methods. Typically, an app creates objects either while the event loop is running or by loading objects from nib files, so this lack of access usually isn’t a problem. However, if you do need to use Cocoa classes within the `main()` function itself (other than to load nib files or to instantiate NSApplication), you should create an `@autorelease` block to contain the code using the classes.

### The Delegate and Notifications

You can assign a delegate to your NSApplication object. The delegate responds to certain messages on behalf of the object. Some of these messages, such as application(_:openFile:), ask the delegate to perform an action. Another message, applicationShouldTerminate(_:), lets the delegate determine whether the app should be allowed to quit. The NSApplication class sends these messages directly to its delegate.

NSApplication also posts notifications to the app’s default notification center. Any object may register to receive one or more of the notifications posted by NSApplication by sending the message addObserver(_:selector:name:object:) to the default notification center (an instance of the `NSNotificationCenter` class). The delegate of NSApplication is automatically registered to receive these notifications if it implements certain delegate methods. For example, NSApplication posts notifications when it’s about to be done launching the app and when it’s done launching the app (willFinishLaunchingNotification and didFinishLaunchingNotification). The delegate has an opportunity to respond to these notifications by implementing the methods applicationWillFinishLaunching(_:) and applicationDidFinishLaunching(_:). If the delegate wants to be informed of both events, it implements both methods. If it needs to know only when the app is finished launching, it implements only applicationDidFinishLaunching(_:).

### System Services

`NSApplication` interacts with the system services architecture to provide services to your app through the Services menu.

### Subclassing Notes

You rarely should find a real need to create a custom `NSApplication` subclass. Unlike some object-oriented libraries, Cocoa doesn’t require you to subclass `NSApplication` to customize app behavior. Instead it gives you many other ways to customize an app. This section discusses both some of the possible reasons to subclass `NSApplication` and some of the reasons *not* to subclass `NSApplication`.

To use a custom subclass of `NSApplication`, send shared to your subclass rather than directly to `NSApplication`. If you create your app in Xcode, you can accomplish this by setting your custom app class to be the principal class. In Xcode, double-click the app target in the Groups and Files list to open the Info window for the target. Then display the Properties pane of the window and replace “NSApplication” in the Principal Class field with the name of your custom class. The `NSApplicationMain` function sends shared to the principal class to obtain the global app instance (`NSApp`)—which in this case will be an instance of your custom subclass of `NSApplication`.

Important

Many AppKit classes rely on the `NSApplication` class and may not work properly until this class is fully initialized. As a result, you should not, for example, attempt to invoke methods of other AppKit classes from an initialization method of an `NSApplication` subclass.

#### Methods to Override

Generally, you subclass `NSApplication` to provide your own special responses to messages that are routinely sent to the global app object (`NSApp`). `NSApplication` doesn’t have primitive methods in the sense of methods that you must override in your subclass. Here are four methods that are possible candidates for overriding:

- Override run() if you want the app to manage the main event loop differently than it does by default. (This a critical and complex task, however, that you should only attempt with good reason).

- Override sendEvent(_:) if you want to change how events are dispatched or perform some special event processing.

- Override requestUserAttention(_:) if you want to modify how your app attracts the attention of the user (for example, offering an alternative to the bouncing app icon in the Dock).

- Override target(forAction:) to substitute another object for the target of an action message.

#### Special Considerations

The global app object uses `@autorelease` blocks in its run() method; if you override this method, you’ll need to create your own `@autorelease` blocks.

Do not override shared. The default implementation, which is essential to app behavior, is too complex to duplicate on your own.

#### Alternatives to Subclassing

`NSApplication` defines numerous Delegation methods that offer opportunities for modifying specific aspects of app behavior. Instead of making a custom subclass of `NSApplication`, your app delegate may be able to implement one or more of these methods to accomplish your design goals. In general, a better design than subclassing `NSApplication` is to put the code that expresses your app’s special behavior into one or more custom objects called controllers. Methods defined in your controllers can be invoked from a small dispatcher object without being closely tied to the global app object.

## Topics

### Getting the Shared App Object

class var shared: NSApplication

Returns the application instance, creating it if it doesn’t exist yet.

var NSApp: NSApplication!

The global variable for the shared app instance.

### Managing the App’s Behavior

var delegate: (any NSApplicationDelegate)?

The app delegate object.

protocol NSApplicationDelegate

A set of methods that manage your app’s life cycle and its interaction with common system services.

### Managing the Event Loop

func nextEvent(matching: NSEvent.EventTypeMask, until: Date?, inMode: RunLoop.Mode, dequeue: Bool) -> NSEvent?

Returns the next event matching a given mask, or `nil` if no such event is found before a specified expiration date.

func discardEvents(matching: NSEvent.EventTypeMask, before: NSEvent?)

Removes all events matching the given mask and generated before the specified event.

var currentEvent: NSEvent?

The last event object that the app retrieved from the event queue.

var isRunning: Bool

A Boolean value indicating whether the main event loop is running.

func run()

Starts the main event loop.

func finishLaunching()

Activates the app, opens any files specified by the `NSOpen` user default, and unhighlights the app’s icon.

func stop(Any?)

Stops the main event loop.

func sendEvent(NSEvent)

Dispatches an event to other objects.

func postEvent(NSEvent, atStart: Bool)

Adds a given event to the receiver’s event queue.

### Posting Actions

func tryToPerform(Selector, with: Any?) -> Bool

Dispatches an action message to the specified target.

func sendAction(Selector, to: Any?, from: Any?) -> Bool

Sends the given action message to the given target.

func target(forAction: Selector) -> Any?

Returns the object that receives the action message specified by the given selector.

func target(forAction: Selector, to: Any?, from: Any?) -> Any?

Searches for an object that can receive the message specified by the given selector.

### Terminating the App

func terminate(Any?)

Terminates the receiver.

func reply(toApplicationShouldTerminate: Bool)

Responds to `NSTerminateLater` once the app knows whether it can terminate.

### Activating and Deactivating the App

Passing control from one app to another with cooperative activation

Request focus for your app, and coordinate passing control from one app to another.

func activate()

Activates the receiver app, if appropriate.

func deactivate()

Deactivates the receiver.

var isActive: Bool

A Boolean value indicating whether this is the active app.

func yieldActivation(to: NSRunningApplication)

Explicitly allows another app to make itself active.

func yieldActivation(toApplicationWithBundleIdentifier: String)

Explicitly allows another app to make itself active.

struct ActivationOptions

The following flags are for activate(options:).

### Managing Relaunch on Login

func disableRelaunchOnLogin()

Disables relaunching the app on login.

func enableRelaunchOnLogin()

Enables relaunching the app on login.

### Managing Remote Notifications

func registerForRemoteNotifications()

Register for notifications sent by Apple Push Notification service (APNs).

func unregisterForRemoteNotifications()

Unregister for notifications received from Apple Push Notification service.

var enabledRemoteNotificationTypes: NSApplication.RemoteNotificationType

The types of push notifications that the app accepts.

func registerForRemoteNotifications(matching: NSApplication.RemoteNotificationType)

Register to receive notifications of the specified types from a provider through the Apple Push Notification service.

Deprecated

var isRegisteredForRemoteNotifications: Bool

A Boolean value indicating whether the app is registered with Apple Push Notification service (APNs).

struct RemoteNotificationType

These constants determine whether apps launched by remote notifications display a badge.

### Managing the App’s Appearance

var appearance: NSAppearance?

The appearance associated with the app’s windows.

var effectiveAppearance: NSAppearance

The appearance that AppKit uses to draw the app’s interface.

var currentSystemPresentationOptions: NSApplication.PresentationOptions

The set of app presentation options that are currently in effect for the system.

var presentationOptions: NSApplication.PresentationOptions

The presentation options that should be in effect for the system when this app is active.

struct PresentationOptions

Constants that control the presentation of the app, typically for fullscreen apps such as games or kiosks.

### Managing Windows, Panels, and Menus

App Windows

Show, hide, minimize, arrange, and update your app’s windows.

Modal Windows and Panels

Display a modal window or show one of the standard app panels, such as the app’s About panel.

Menus

Access the app’s main menu items and update the window and services menus.

### User Interface Layout Direction

var userInterfaceLayoutDirection: NSUserInterfaceLayoutDirection

The layout direction of the user interface.

enum NSUserInterfaceLayoutDirection

Specifies the directional flow of the user interface.

### Accessing the Dock Tile

var dockTile: NSDockTile

The app’s Dock tile.

var applicationIconImage: NSImage!

The image used for the app’s icon.

### Customizing the Touch Bar

func toggleTouchBarCustomizationPalette(Any?)

Show or hides the interface for customizing the Touch Bar.

### Managing User Attention Requests

func requestUserAttention(NSApplication.RequestUserAttentionType) -> Int

Starts a user attention request.

enum RequestUserAttentionType

These constants specify the level of severity of a user attention request and are used by cancelUserAttentionRequest(_:) and requestUserAttention(_:).

func cancelUserAttentionRequest(Int)

Cancels a previous user attention request.

func reply(toOpenOrPrint: NSApplication.DelegateReply)

Handles errors that might occur when the user attempts to open or print files.

enum DelegateReply

Constants that indicate whether a copy or print operation was successful, was canceled, or failed.

### Providing Help Information

func registerUserInterfaceItemSearchHandler(any NSUserInterfaceItemSearching)

Register an object that provides help data to your app.

func searchString(String, inUserInterfaceItemString: String, range: NSRange, found: UnsafeMutablePointer&lt;NSRange>?) -> Bool

Searches for the string in the user interface.

func unregisterUserInterfaceItemSearchHandler(any NSUserInterfaceItemSearching)

Unregister an object that provides help data to your app.

func showHelp(Any?)

If your project is properly registered, and the necessary keys have been set in the property list, this method launches Help Viewer and displays the first page of your app’s help book.

func activateContextHelpMode(Any?)

Places the receiver in context-sensitive help mode.

var helpMenu: NSMenu?

The help menu used by the app.

### Providing Services

func validRequestor(forSendType: NSPasteboard.PasteboardType?, returnType: NSPasteboard.PasteboardType?) -> Any?

Indicates whether the receiver can send and receive the specified pasteboard types.

var servicesProvider: Any?

The object that provides the services the current app advertises in the Services menu of other apps.

### Determining Access to the Keyboard

var isFullKeyboardAccessEnabled: Bool

A Boolean value indicating whether Full Keyboard Access is enabled in the Keyboard preference pane.

### Hiding Apps

func hideOtherApplications(Any?)

Hides all apps, except the receiver.

func unhideAllApplications(Any?)

Unhides all apps, including the receiver.

### Managing Threads

class func detachDrawingThread(Selector, toTarget: Any, with: Any?)

Creates and executes a new thread based on the specified target and selector.

### Logging Exceptions

func reportException(NSException)

Logs a given exception by calling `NSLog()`.

### Configuring the Activation Policy

func activationPolicy() -> NSApplication.ActivationPolicy

Returns the app’s activation policy.

func setActivationPolicy(NSApplication.ActivationPolicy) -> Bool

Attempts to modify the app’s activation policy.

enum ActivationPolicy

Activation policies (used by activationPolicy) that control whether and how an app may be activated.

### Scripting Your App

var orderedDocuments: [NSDocument]

An array of document objects arranged according to the front-to-back ordering of their associated windows.

var orderedWindows: [NSWindow]

An array of window objects arranged according to their front-to-back ordering on the screen.

### Notifications

These notifications apply to `NSApplication`. See Notifications in NSWorkspace for additional, similar notifications.

class let didBecomeActiveNotification: NSNotification.Name

Posted immediately after the app becomes active.

class let didChangeScreenParametersNotification: NSNotification.Name

Posted when the configuration of the displays attached to the computer is changed.

class let didFinishLaunchingNotification: NSNotification.Name

Posted at the end of the finishLaunching() method to indicate that the app has completed launching and is ready to run.

class let didHideNotification: NSNotification.Name

Posted at the end of the hide(_:) method to indicate that the app is now hidden.

class let didResignActiveNotification: NSNotification.Name

Posted immediately after the app gives up its active status to another app.

class let didUnhideNotification: NSNotification.Name

Posted at the end of the unhideWithoutActivation() method to indicate that the app is now visible.

class let didUpdateNotification: NSNotification.Name

Posted at the end of the updateWindows() method to indicate that the app has finished updating its windows.

class let willBecomeActiveNotification: NSNotification.Name

Posted immediately before the app becomes active.

class let willFinishLaunchingNotification: NSNotification.Name

Posted at the start of the finishLaunching() method to indicate that the app has completed its initialization process and is about to finish launching.

class let willHideNotification: NSNotification.Name

Posted at the start of the hide(_:) method to indicate that the app is about to be hidden.

class let willResignActiveNotification: NSNotification.Name

Posted immediately before the app gives up its active status to another app.

class let willTerminateNotification: NSNotification.Name

Sends a notification to termintate the app.

class let willUnhideNotification: NSNotification.Name

Posted at the start of the unhideWithoutActivation() method to indicate that the app is about to become visible.

class let willUpdateNotification: NSNotification.Name

Posted at the start of the updateWindows() method to indicate that the app is about to update its windows.

class let didFinishRestoringWindowsNotification: NSNotification.Name

Posted when the app has finished restoring windows.

class let didChangeOcclusionStateNotification: NSNotification.Name

Posted when the app’s occlusion state changes.

### Loading Cocoa Bundles

static func loadApplication()

### Deprecated

Avoid using deprecated classes and protocols in your apps.

Deprecated Symbols

Review symbols that are no longer supported, and find the replacements to use instead.

## Relationships

### Inherits From

- NSResponder

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAppearanceCustomization
- NSCoding
- NSMenuItemValidation
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceValidations

## See Also

### Life Cycle

class NSRunningApplication

An object that can manipulate and provide information for a single instance of an app.

protocol NSApplicationDelegate

A set of methods that manage your app’s life cycle and its interaction with common system services.

func NSApplicationMain(Int32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>) -> Int32

Called by the main function to create and run the application.

