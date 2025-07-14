

- AppKit
- NSApplicationDelegate
-  applicationWillBecomeActive(\_:) 

Instance Method

# applicationWillBecomeActive(\_:)

Tells the delegate that the app is about to become active.

macOS 10.10+

``` source
@MainActor
optional func applicationWillBecomeActive(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named willBecomeActiveNotification. Calling the object method of this notification returns the `NSApplication` object itself.

## See Also

### Related Documentation

func applicationWillFinishLaunching(Notification)

Tells the delegate that the app’s initialization is about to complete.

### Managing Active Status

func applicationDidBecomeActive(Notification)

Tells the delegate that the app is now active.

func applicationWillResignActive(Notification)

Tells the delegate that the app is about to become inactive and will lose focus.

func applicationDidResignActive(Notification)

Tells the delegate that the app is no longer active and doesn’t have focus.

