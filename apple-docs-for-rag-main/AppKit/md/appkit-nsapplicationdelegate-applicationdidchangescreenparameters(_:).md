

- AppKit
- NSApplicationDelegate
-  applicationDidChangeScreenParameters(\_:) 

Instance Method

# applicationDidChangeScreenParameters(\_:)

Tells the delegate about changes to the configuration of any attached displays.

macOS 10.10+

``` source
@MainActor
optional func applicationDidChangeScreenParameters(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didChangeScreenParametersNotification. Calling the object method of this notification returns the `NSApplication` object itself.

