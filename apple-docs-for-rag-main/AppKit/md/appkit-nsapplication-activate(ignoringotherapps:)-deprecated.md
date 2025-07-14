

- AppKit
- NSApplication
-  activate(ignoringOtherApps:) Deprecated

Instance Method

# activate(ignoringOtherApps:)

Makes the receiver the active app.

macOS 10.0–15.4Deprecated

``` source
@MainActor
func activate(ignoringOtherApps ignoreOtherApps: Bool)
```

Deprecated

Use NSApplication method activate() instead.

## Parameters 

`ignoreOtherApps`  

If false, the app activates only if no other app is currently active. If true, the app activates regardless.

## Discussion

The `flag` parameter is normally set to false. When the Finder launches an app, using a value of false for `flag` allows the app to become active if the user waits for it to launch, but the app remains unobtrusive if the user activates another app. Regardless of the setting of `flag`, there may be a time lag before the app activates—you shouldn’t assume the app will be active immediately after sending this message.

You rarely need to invoke this method. Under most circumstances, AppKit takes care of proper activation. However, you might find this method useful if you implement your own methods for inter-app communication.

You don’t need to send this message to make one of the app’s `NSWindows` key. When you send a makeKey() message to an `NSWindow` object, you ensure that it’s the key window when the app is active.

## See Also

### Related Documentation

func deactivate()

Deactivates the receiver.

var isActive: Bool

A Boolean value indicating whether this is the active app.

### Methods

func endModalSession(NSApplication.ModalSession)

Finishes a modal session.

func beginSheet(NSWindow, modalFor: NSWindow, modalDelegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer!)

Starts a document modal session.

Deprecated

func endSheet(NSWindow)

Ends a document modal session by specifying the sheet window.

Deprecated

func endSheet(NSWindow, returnCode: Int)

Ends a document modal session by specifying the sheet window.

Deprecated

