

- AppKit
- NSApplicationDelegate
-  applicationDidResignActive(\_:) 

Instance Method

# applicationDidResignActive(\_:)

Tells the delegate that the app is no longer active and doesn’t have focus.

macOS 10.10+

``` source
@MainActor
optional func applicationDidResignActive(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didResignActiveNotification. Calling the object method of this notification returns the `NSApplication` object itself.

## See Also

### Managing Active Status

func applicationWillBecomeActive(Notification)

Tells the delegate that the app is about to become active.

func applicationDidBecomeActive(Notification)

Tells the delegate that the app is now active.

func applicationWillResignActive(Notification)

Tells the delegate that the app is about to become inactive and will lose focus.

