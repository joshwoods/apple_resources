

- AppKit
- NSApplicationDelegate
-  applicationShouldTerminate(\_:) 

Instance Method

# applicationShouldTerminate(\_:)

Returns a value that indicates if the app should terminate.

macOS

``` source
@MainActor
optional func applicationShouldTerminate(_ sender: NSApplication) -> NSApplication.TerminateReply
```

## Parameters 

`sender`  

The application object that is about to be terminated.

## Return Value

One of the values defined in NSApplication.TerminateReply constants indicating whether the application should terminate. For compatibility reasons, a return value of false is equivalent to NSApplication.TerminateReply.terminateCancel, and a return value of true is equivalent to NSApplication.TerminateReply.terminateNow.

## Discussion

This method is called after the application’s Quit menu item has been selected, or after the terminate(_:) method has been called. Generally, you should return NSApplication.TerminateReply.terminateNow to allow the termination to complete, but you can cancel the termination process or delay it somewhat as needed. For example, you might delay termination to finish processing some critical data but then terminate the application as soon as you are done by calling the reply(toApplicationShouldTerminate:) method.

## See Also

### Related Documentation

func terminate(Any?)

Terminates the receiver.

### Terminating Applications

enum TerminateReply

Constants that determine whether an app should terminate.

func applicationShouldTerminateAfterLastWindowClosed(NSApplication) -> Bool

Returns a Boolean value that indicates if the app terminates once the last window closes.

func applicationWillTerminate(Notification)

Tells the delegate that the app is about to terminate.

