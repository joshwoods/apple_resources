

- AppKit
- NSApplicationDelegate
-  applicationWillTerminate(\_:) 

Instance Method

# applicationWillTerminate(\_:)

Tells the delegate that the app is about to terminate.

macOS 10.10+

``` source
@MainActor
optional func applicationWillTerminate(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named willTerminateNotification. Calling the object method of this notification returns the `NSApplication` object itself.

## Discussion

Your delegate can use this method to perform any final cleanup before the app terminates. The app will terminate after this method returns.

Note

This method isn’t called during sudden termination of an app. For more information about sudden termination, see the section ProcessInfo of ProcessInfo.

## See Also

### Related Documentation

func terminate(Any?)

Terminates the receiver.

### Terminating Applications

func applicationShouldTerminate(NSApplication) -> NSApplication.TerminateReply

Returns a value that indicates if the app should terminate.

enum TerminateReply

Constants that determine whether an app should terminate.

func applicationShouldTerminateAfterLastWindowClosed(NSApplication) -> Bool

Returns a Boolean value that indicates if the app terminates once the last window closes.

