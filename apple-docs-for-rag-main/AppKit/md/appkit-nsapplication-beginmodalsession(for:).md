

- AppKit
- NSApplication
-  beginModalSession(for:) 

Instance Method

# beginModalSession(for:)

Sets up a modal session with the given window and returns a pointer to the `NSModalSession` structure representing the session.

macOS

``` source
@MainActor
func beginModalSession(for window: NSWindow) -> NSApplication.ModalSession
```

## Parameters 

`window`  

The window for the session.

## Return Value

A pointer to the `NSModalSession` structure that represents the session.

## Discussion

In a modal session, the app receives mouse events only if they occur in `aWindow`. The window is made key, and if not already visible is placed onscreen using the `NSWindow` method center().

The beginModalSession(for:) method only sets up the modal session. To actually run the session, use runModalSession(_:). beginModalSession(for:) should be balanced by endModalSession(_:). Make sure these two messages are sent within the same exception-handling scope. That is, if you send beginModalSession(for:) inside an `NS_DURING` construct, you must send endModalSession(_:) before `NS_ENDHANDLER`.

If an exception is raised, beginModalSession(for:) arranges for proper cleanup. Do not use `NS_DURING` constructs to send an endModalSession(_:) message in the event of an exception.

A loop using these methods is similar to a modal event loop run with runModal(for:), except the app can continue processing between method invocations.

## See Also

### Running a Modal Window

func runModal(for: NSWindow) -> NSApplication.ModalResponse

Starts a modal event loop for the specified window.

func stopModal()

Stops a modal event loop.

func stopModal(withCode: NSApplication.ModalResponse)

Stops a modal event loop, allowing you to return a custom result code.

func abortModal()

Aborts the event loop started by runModal(for:) or runModalSession(_:).

func runModalSession(NSApplication.ModalSession) -> NSApplication.ModalResponse

Runs a given modal session, as defined in a previous invocation of beginModalSession(for:).

var modalWindow: NSWindow?

The modal window displayed by the app.

struct ModalResponse

A set of button return values for modal dialogs.

typealias ModalSession

Variables of type `NSModalSession` point to information used by the system between `NSApplication`’s beginModalSession(for:) and endModalSession(_:) messages.

