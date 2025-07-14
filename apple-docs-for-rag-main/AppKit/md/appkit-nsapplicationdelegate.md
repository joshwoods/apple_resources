

- AppKit
-  NSApplicationDelegate 

Protocol

# NSApplicationDelegate

A set of methods that manage your app’s life cycle and its interaction with common system services.

macOS

``` source
protocol NSApplicationDelegate : NSObjectProtocol
```

## Topics

### Launching Applications

func applicationWillFinishLaunching(Notification)

Tells the delegate that the app’s initialization is about to complete.

func applicationDidFinishLaunching(Notification)

Tells the delegate that the app’s initialization is complete but it hasn’t received its first event.

NSApplicationDidFinishLaunching User Info Keys

The keys you use to access values in the launch options dictionary that the system passes to your app at initialization.

### Managing Active Status

func applicationWillBecomeActive(Notification)

Tells the delegate that the app is about to become active.

func applicationDidBecomeActive(Notification)

Tells the delegate that the app is now active.

func applicationWillResignActive(Notification)

Tells the delegate that the app is about to become inactive and will lose focus.

func applicationDidResignActive(Notification)

Tells the delegate that the app is no longer active and doesn’t have focus.

### Terminating Applications

func applicationShouldTerminate(NSApplication) -> NSApplication.TerminateReply

Returns a value that indicates if the app should terminate.

enum TerminateReply

Constants that determine whether an app should terminate.

func applicationShouldTerminateAfterLastWindowClosed(NSApplication) -> Bool

Returns a Boolean value that indicates if the app terminates once the last window closes.

func applicationWillTerminate(Notification)

Tells the delegate that the app is about to terminate.

### Hiding Applications

func applicationWillHide(Notification)

Tells the delegate that the app is about to be hidden.

func applicationDidHide(Notification)

Tells the delegate that the app is now hidden.

func applicationWillUnhide(Notification)

Tells the delegate that the app is about to become visible.

func applicationDidUnhide(Notification)

Tells the delegate that the app is now visible.

### Managing Windows

func applicationWillUpdate(Notification)

Tells the delegate that the app is about to update its windows.

func applicationDidUpdate(Notification)

Tells the delegate that the app’s windows did update.

func applicationShouldHandleReopen(NSApplication, hasVisibleWindows: Bool) -> Bool

Returns a Boolean value that indicates if the app responds to reopen AppleEvents.

### Managing the Dock Menu

func applicationDockMenu(NSApplication) -> NSMenu?

Returns the app’s dock menu.

### Localizing Keyboard Shortcuts

func applicationShouldAutomaticallyLocalizeKeyEquivalents(NSApplication) -> Bool

Returns a Boolean value that tells the system whether to remap menu shortcuts to support localized keyboards.

### Displaying Errors

func application(NSApplication, willPresentError: any Error) -> any Error

Returns an error for the app to display to the user.

### Managing the Screen

func applicationDidChangeScreenParameters(Notification)

Tells the delegate about changes to the configuration of any attached displays.

### Continuing User Activities

func application(NSApplication, willContinueUserActivityWithType: String) -> Bool

Returns a Boolean value that indicates if the app can continue the specified activity.

func application(NSApplication, continue: NSUserActivity, restorationHandler: ([any NSUserActivityRestoring]) -> Void) -> Bool

Returns a Boolean value that indicates if the app successfully recreates the specified activity.

func application(NSApplication, didFailToContinueUserActivityWithType: String, error: any Error)

Tells the delegate that the app couldn’t continue the specified activity.

func application(NSApplication, didUpdate: NSUserActivity)

Tells the delegate that there are changes to the specified activity.

### Handling Push Notifications

func application(NSApplication, didRegisterForRemoteNotificationsWithDeviceToken: Data)

Tells the delegate that the app registered for Apple Push Services.

func application(NSApplication, didFailToRegisterForRemoteNotificationsWithError: any Error)

Tells the delegate that the app was unable to register for Apple Push Services.

func application(NSApplication, didReceiveRemoteNotification: [String : Any])

Tells the delegate when the app receives a remote notification.

### Handling CloudKit Invitations

func application(NSApplication, userDidAcceptCloudKitShareWith: CKShareMetadata)

Tells the delegate when the user accepts a CloudKit sharing invitation.

### Handling SiriKit Intents

func application(NSApplication, handlerFor: INIntent) -> Any?

Returns an intent handler that’s capable of handling the specified intent.

### Opening Files

func application(NSApplication, open: [URL])

Tells the delegate to open the resource at the specified URL.

func application(NSApplication, openFile: String) -> Bool

Returns a Boolean value that indicates if the app opens the specified file.

func application(Any, openFileWithoutUI: String) -> Bool

Returns a Boolean value that indicates if the app opens the specified file without showing its user interface.

func application(NSApplication, openTempFile: String) -> Bool

Returns a Boolean value that indicates if the app opens the specified temporary file.

func application(NSApplication, openFiles: [String])

Tells the delegate to open the specified files.

func applicationShouldOpenUntitledFile(NSApplication) -> Bool

Returns a Boolean value that indicates if the app can open an untitled file.

func applicationOpenUntitledFile(NSApplication) -> Bool

Returns a Boolean value that indicates if the app opens an untitled file.

### Printing

func application(NSApplication, printFile: String) -> Bool

Returns a Boolean value that indicates if the app prints the specified file in its entirety.

func application(NSApplication, printFiles: [String], withSettings: [NSPrintInfo.AttributeKey : Any], showPrintPanels: Bool) -> NSApplication.PrintReply

Returns a value that indicates if the app prints the specified files.

enum PrintReply

Constants that indicate the outcome of a print request.

### Restoring Application State

func applicationSupportsSecureRestorableState(NSApplication) -> Bool

Returns a Boolean value that indicates if the app supports secure state restoration.

func applicationProtectedDataDidBecomeAvailable(Notification)

Tells the delegate that protected data is now available.

func applicationProtectedDataWillBecomeUnavailable(Notification)

Tells the delegate that protected data is about to become unavailable.

func application(NSApplication, willEncodeRestorableState: NSCoder)

Tells the delegate that the app is about to encode its restorable state.

func application(NSApplication, didDecodeRestorableState: NSCoder)

Tells the delegate when the app finished decoding its restorable state.

### Handling Changes to the Occlusion State

func applicationDidChangeOcclusionState(Notification)

Tells the delegate about changes to the app’s occlusion state.

### Scripting Your App

func application(NSApplication, delegateHandlesKey: String) -> Bool

Returns a Boolean value that indicates if the app supports the specified scripting key.

### Type Methods

static func main()

Provides the top-level entry point for the app.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Life Cycle

class NSApplication

An object that manages an app’s main event loop and resources used by all of that app’s objects.

class NSRunningApplication

An object that can manipulate and provide information for a single instance of an app.

func NSApplicationMain(Int32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>) -> Int32

Called by the main function to create and run the application.

