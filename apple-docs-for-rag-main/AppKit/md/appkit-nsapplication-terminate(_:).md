

- AppKit
- NSApplication
-  terminate(\_:) 

Instance Method

# terminate(\_:)

Terminates the receiver.

macOS

``` source
@MainActor
func terminate(_ sender: Any?)
```

## Parameters 

`sender`  

Typically, this parameter contains the object that initiated the termination request.

## Discussion

This method is typically invoked when the user chooses Quit or Exit from the app’s menu.

When invoked, this method performs several steps to process the termination request. First, it asks the app’s document controller (if one exists) to save any unsaved changes in its documents. During this process, the document controller can cancel termination in response to input from the user. If the document controller doesn’t cancel the operation, this method then calls the delegate’s applicationShouldTerminate(_:) method. If applicationShouldTerminate(_:) returns NSApplication.TerminateReply.terminateCancel, the termination process is aborted and control is handed back to the main event loop. If the method returns NSApplication.TerminateReply.terminateLater, the app runs its run loop in the NSModalPanelRunLoopMode mode until the reply(toApplicationShouldTerminate:) method is called with the value true or false. If the applicationShouldTerminate(_:) method returns NSApplication.TerminateReply.terminateNow, this method posts a willTerminateNotification notification to the default notification center.

Don’t bother to put final cleanup code in your app’s `main()` function—it will never be executed. If cleanup is necessary, perform that cleanup in the delegate’s applicationWillTerminate(_:) method.

## See Also

### Related Documentation

func stop(Any?)

Stops the main event loop.

func applicationShouldTerminate(NSApplication) -> NSApplication.TerminateReply

Returns a value that indicates if the app should terminate.

func run()

Starts the main event loop.

func applicationWillTerminate(Notification)

Tells the delegate that the app is about to terminate.

class let willTerminateNotification: NSNotification.Name

Sends a notification to termintate the app.

### Terminating the App

func reply(toApplicationShouldTerminate: Bool)

Responds to `NSTerminateLater` once the app knows whether it can terminate.

