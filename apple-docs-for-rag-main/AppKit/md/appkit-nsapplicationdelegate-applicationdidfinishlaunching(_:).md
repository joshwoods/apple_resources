

- AppKit
- NSApplicationDelegate
-  applicationDidFinishLaunching(\_:) 

Instance Method

# applicationDidFinishLaunching(\_:)

Tells the delegate that the app’s initialization is complete but it hasn’t received its first event.

macOS 10.10+

``` source
@MainActor
optional func applicationDidFinishLaunching(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didFinishLaunchingNotification. Calling the object method of this notification returns the `NSApplication` object itself.

## Discussion

Delegates can implement this method to perform further initialization. This method is called after the application’s main run loop has been started but before it has processed any events. If the application was launched by the user opening a file, the delegate’s application(_:openFile:) method is called before this method. If you want to perform initialization before any files are opened, implement the applicationWillFinishLaunching(_:) method in your delegate, which is called before application(_:openFile:).)

## See Also

### Related Documentation

func finishLaunching()

Activates the app, opens any files specified by the `NSOpen` user default, and unhighlights the app’s icon.

func application(NSApplication, openFile: String) -> Bool

Returns a Boolean value that indicates if the app opens the specified file.

func applicationDidBecomeActive(Notification)

Tells the delegate that the app is now active.

### Launching Applications

func applicationWillFinishLaunching(Notification)

Tells the delegate that the app’s initialization is about to complete.

NSApplicationDidFinishLaunching User Info Keys

The keys you use to access values in the launch options dictionary that the system passes to your app at initialization.

