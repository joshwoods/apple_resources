

- AppKit
- NSApplicationDelegate
-  applicationWillFinishLaunching(\_:) 

Instance Method

# applicationWillFinishLaunching(\_:)

Tells the delegate that the app’s initialization is about to complete.

macOS 10.10+

``` source
@MainActor
optional func applicationWillFinishLaunching(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named willFinishLaunchingNotification. Calling the object method of this notification returns the `NSApplication` object itself.

## Mentioned in 

Supporting Continuity Camera in Your Mac App

## See Also

### Related Documentation

func applicationWillBecomeActive(Notification)

Tells the delegate that the app is about to become active.

Sheet Programming Topics

func finishLaunching()

Activates the app, opens any files specified by the `NSOpen` user default, and unhighlights the app’s icon.

Services Implementation Guide

Mac App Programming Guide

Local and Remote Notification Programming Guide

Notification Programming Topics

### Launching Applications

func applicationDidFinishLaunching(Notification)

Tells the delegate that the app’s initialization is complete but it hasn’t received its first event.

NSApplicationDidFinishLaunching User Info Keys

The keys you use to access values in the launch options dictionary that the system passes to your app at initialization.

