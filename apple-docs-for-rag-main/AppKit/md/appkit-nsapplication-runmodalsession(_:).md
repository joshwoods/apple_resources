

- AppKit
- NSApplication
-  runModalSession(\_:) 

Instance Method

# runModalSession(\_:)

Runs a given modal session, as defined in a previous invocation of beginModalSession(for:).

macOS

``` source
@MainActor
func runModalSession(_ session: NSApplication.ModalSession) -> NSApplication.ModalResponse
```

## Parameters 

`session`  

A pointer to the modal session structure returned by the beginModalSession(for:) method for the window to be displayed.

## Return Value

An integer indicating the reason that this method returned. See the discussion for a description of possible return values.

## Discussion

A loop that uses this method is similar in some ways to a modal event loop run with runModal(for:), except with this method your code can do some additional work between method invocations. When you invoke this method, events for the `NSWindow` object of this session are dispatched as normal. This method returns when there are no more events. You must invoke this method frequently enough in your loop that the window remains responsive to events. However, you should not invoke this method in a tight loop because it returns immediately if there are no events, and consequently you could end up polling for events rather than blocking.

Typically, you use this method in situations where you want to do some additional processing on the current thread while the modal loop runs. For example, while processing a large data set, you might want to use a modal dialog to display progress and give the user a chance to cancel the operation. If you want to display a modal dialog and do not need to do any additional work in parallel, use runModal(for:) instead. When there are no pending events, that method waits idly instead of consuming CPU time.

The following code shows a sample loop you can use in your code:

```
NSModalSession session = [NSApp beginModalSessionForWindow:theWindow];
for (;;) {
    if ([NSApp runModalSession:session] != NSModalResponseContinue)
        break;
    [self doSomeWork];
}
[NSApp endModalSession:session];
```

If the modal session was not stopped, this method returns `NSModalResponseContinue`. At this point, your app can do some work before the next invocation of runModalSession(_:) (as indicated in the example’s `doSomeWork` call). If stopModal() was invoked as the result of event processing, runModalSession(_:) returns `NSModalResponseStop`. If stopModal(withCode:) was invoked, this method returns the value passed to stopModal(withCode:). If abortModal() was invoked, this method returns `NSModalResponseAbort`.

The window is placed on the screen and made key as a result of the runModalSession(_:) message. Do not send a separate makeKeyAndOrderFront(_:) message.

## See Also

### Related Documentation

func endModalSession(NSApplication.ModalSession)

Finishes a modal session.

func run()

Starts the main event loop.

### Running a Modal Window

func runModal(for: NSWindow) -> NSApplication.ModalResponse

Starts a modal event loop for the specified window.

func stopModal()

Stops a modal event loop.

func stopModal(withCode: NSApplication.ModalResponse)

Stops a modal event loop, allowing you to return a custom result code.

func abortModal()

Aborts the event loop started by runModal(for:) or runModalSession(_:).

func beginModalSession(for: NSWindow) -> NSApplication.ModalSession

Sets up a modal session with the given window and returns a pointer to the `NSModalSession` structure representing the session.

var modalWindow: NSWindow?

The modal window displayed by the app.

struct ModalResponse

A set of button return values for modal dialogs.

typealias ModalSession

Variables of type `NSModalSession` point to information used by the system between `NSApplication`’s beginModalSession(for:) and endModalSession(_:) messages.

