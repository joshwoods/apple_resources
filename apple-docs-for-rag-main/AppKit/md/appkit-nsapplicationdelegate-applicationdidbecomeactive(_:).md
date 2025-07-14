

- AppKit
- NSApplicationDelegate
-  applicationDidBecomeActive(\_:) 

Instance Method

# applicationDidBecomeActive(\_:)

Tells the delegate that the app is now active.

macOS 10.10+

``` source
@MainActor
optional func applicationDidBecomeActive(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didBecomeActiveNotification. Calling the object method of this notification returns the `NSApplication` object itself.

## See Also

### Related Documentation

func applicationDidFinishLaunching(Notification)

Tells the delegate that the app’s initialization is complete but it hasn’t received its first event.

### Managing Active Status

func applicationWillBecomeActive(Notification)

Tells the delegate that the app is about to become active.

func applicationWillResignActive(Notification)

Tells the delegate that the app is about to become inactive and will lose focus.

func applicationDidResignActive(Notification)

Tells the delegate that the app is no longer active and doesn’t have focus.

