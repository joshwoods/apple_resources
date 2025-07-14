

- AppKit
- NSApplication
-  runModal(for:) 

Instance Method

# runModal(for:)

Starts a modal event loop for the specified window.

macOS

``` source
@MainActor
func runModal(for window: NSWindow) -> NSApplication.ModalResponse
```

## Parameters 

`window`  

The window to be displayed modally. If it is not already visible, the window is centered on the screen using the value in its center() method and made visible and key. If it is already visible, it is simply made key.

## Return Value

An integer indicating the reason that this method returned. See NSApplication.ModalResponse possible return values.

## Discussion

This method runs a modal event loop for the specified window synchronously. It displays the specified window, makes it key, starts the run loop, and processes events for that window. (You do not need to show the window yourself.) While the app is in that loop, it does not respond to any other events (including mouse, keyboard, or window-close events) unless they are associated with the window. It also does not perform any tasks (such as firing timers) that are not associated with the modal run loop. In other words, this method consumes only enough CPU time to process events and dispatch them to the action methods associated with the modal window.

You can exit the modal loop by calling the stopModal(), stopModal(withCode:), or abortModal() methods from your modal window code. If you use the stopModal(withCode:) method to stop the modal event loop, this method returns the argument passed to stopModal(withCode:). If you use stopModal() instead, this method returns the constant stop. If you use abortModal(), this method returns the constant abort.

## See Also

### Related Documentation

func run()

Starts the main event loop.

### Running a Modal Window

func stopModal()

Stops a modal event loop.

func stopModal(withCode: NSApplication.ModalResponse)

Stops a modal event loop, allowing you to return a custom result code.

func abortModal()

Aborts the event loop started by runModal(for:) or runModalSession(_:).

func beginModalSession(for: NSWindow) -> NSApplication.ModalSession

Sets up a modal session with the given window and returns a pointer to the `NSModalSession` structure representing the session.

func runModalSession(NSApplication.ModalSession) -> NSApplication.ModalResponse

Runs a given modal session, as defined in a previous invocation of beginModalSession(for:).

var modalWindow: NSWindow?

The modal window displayed by the app.

struct ModalResponse

A set of button return values for modal dialogs.

typealias ModalSession

Variables of type `NSModalSession` point to information used by the system between `NSApplication`’s beginModalSession(for:) and endModalSession(_:) messages.

