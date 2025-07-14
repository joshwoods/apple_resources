

- AppKit
-  NSRunningApplication 

Class

# NSRunningApplication

An object that can manipulate and provide information for a single instance of an app.

macOS 10.6+

``` source
class NSRunningApplication
```

## Mentioned in 

Passing control from one app to another with cooperative activation

## Overview

Some properties of an app are fixed, such as the bundle identifier. Other properties may vary over time, such as whether the app is hidden. Properties that vary can be observed with key-value observing, in which case the description comment for the method notes this capability.

Properties that vary over time are inherently race-prone. For example, a hidden app may unhide itself at any time. To ameliorate this, properties persist until the next turn of the main run loop in a common mode. For example, if you repeatedly poll an unhidden app for its hidden property without allowing the run loop to run, it will continue to return false, even if the app hides, until the next turn of the run loop.

NSRunningApplication is thread safe, in that its properties are returned atomically. However, it is still subject to the main run loop policy described above. If you access an instance of NSRunningApplication from a background thread, be aware that its time-varying properties may change from under you as the main run loop runs (or not).

An NSRunningApplication instance remains valid after the app exits. However, most properties lose their significance, and some properties may not be available on a terminated application.

To access the list of all running apps, use the runningApplications method in NSWorkspace.

## Topics

### Getting running application instances

convenience init?(processIdentifier: pid_t)

Returns the running application with the given process identifier, or nil if no application has that pid.

class func runningApplications(withBundleIdentifier: String) -> [NSRunningApplication]

Returns an array of currently running applications with the specified bundle identifier.

class var current: NSRunningApplication

Returns an `NSRunningApplication` representing this application.

### Activating applications

func activate(options: NSApplication.ActivationOptions) -> Bool

Attempts to activate the application using the specified options.

func activate(from: NSRunningApplication, options: NSApplication.ActivationOptions) -> Bool

Attempts to activate the application using the specified options.

var isActive: Bool

Indicates whether the application is currently frontmost.

struct ActivationOptions

The following flags are for activate(options:).

var activationPolicy: NSApplication.ActivationPolicy

Indicates the activation policy of the application.

enum ActivationPolicy

Activation policies (used by activationPolicy) that control whether and how an app may be activated.

### Hiding and unhiding applications

func hide() -> Bool

Attempts to hide or the application.

func unhide() -> Bool

Attempts to unhide or the application.

var isHidden: Bool

Indicates whether the application is currently hidden.

### Application information

var localizedName: String?

Indicates the localized name of the application.

var icon: NSImage?

Returns the icon for the receiver’s application.

var bundleIdentifier: String?

Indicates the `CFBundleIdentifier` of the application.

var bundleURL: URL?

Indicates the URL to the application’s bundle.

var executableArchitecture: Int

Indicates the executing processor architecture for the application.

var executableURL: URL?

Indicates the URL to the application’s executable.

var launchDate: Date?

Indicates the date when the application was launched.

var isFinishedLaunching: Bool

Indicates whether the receiver’s process has finished launching,

var processIdentifier: pid_t

Indicates the process identifier (pid) of the application.

var ownsMenuBar: Bool

Returns whether the application owns the current menu bar.

### Terminating applications

func forceTerminate() -> Bool

Attempts to force the receiver to quit.

func terminate() -> Bool

Attempts to quit the receiver normally.

var isTerminated: Bool

Indicates that the receiver’s application has terminated.

class func terminateAutomaticallyTerminableApplications()

Terminates invisibly running applications as if triggered by system memory pressure.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Life Cycle

class NSApplication

An object that manages an app’s main event loop and resources used by all of that app’s objects.

protocol NSApplicationDelegate

A set of methods that manage your app’s life cycle and its interaction with common system services.

func NSApplicationMain(Int32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>) -> Int32

Called by the main function to create and run the application.

