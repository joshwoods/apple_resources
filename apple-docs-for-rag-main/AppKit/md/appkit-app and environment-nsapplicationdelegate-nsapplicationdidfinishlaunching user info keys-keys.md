

- AppKit
- App and Environment
- NSApplicationDelegate
-  NSApplicationDidFinishLaunching User Info Keys 

API Collection

# NSApplicationDidFinishLaunching User Info Keys

The keys you use to access values in the launch options dictionary that the system passes to your app at initialization.

## Topics

### Keys

class let launchIsDefaultUserInfoKey: String

The value for this key is an `NSNumber` containing a Boolean value. The value is false if the app was launched to open or print a file, to perform a Service action, if the app had saved state that will be restored, or if the app launch was in some other sense not a default launch. Otherwise its value will be true.

class let launchUserNotificationUserInfoKey: String

A key that indicates your app was launched because a user activated a notification in the Notification Center.

## See Also

### Launching Applications

func applicationWillFinishLaunching(Notification)

Tells the delegate that the app’s initialization is about to complete.

func applicationDidFinishLaunching(Notification)

Tells the delegate that the app’s initialization is complete but it hasn’t received its first event.

