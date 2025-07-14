

- AppKit
- NSApplicationDelegate
-  applicationShouldTerminateAfterLastWindowClosed(\_:) 

Instance Method

# applicationShouldTerminateAfterLastWindowClosed(\_:)

Returns a Boolean value that indicates if the app terminates once the last window closes.

macOS

``` source
@MainActor
optional func applicationShouldTerminateAfterLastWindowClosed(_ sender: NSApplication) -> Bool
```

## Parameters 

`sender`  

The application object whose last window was closed.

## Return Value

false if the application should not be terminated when its last window is closed; otherwise, true to terminate the application.

## Discussion

The application sends this message to your delegate when the application’s last window is closed. It sends this message regardless of whether there are still panels open. (A panel in this case is defined as being an instance of `NSPanel` or one of its subclasses.)

If your implementation returns false, control returns to the main event loop and the application is not terminated. If you return true, your delegate’s applicationShouldTerminate(_:) method is subsequently invoked to confirm that the application should be terminated.

## See Also

### Related Documentation

func terminate(Any?)

Terminates the receiver.

### Terminating Applications

func applicationShouldTerminate(NSApplication) -> NSApplication.TerminateReply

Returns a value that indicates if the app should terminate.

enum TerminateReply

Constants that determine whether an app should terminate.

func applicationWillTerminate(Notification)

Tells the delegate that the app is about to terminate.

