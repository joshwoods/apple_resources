

- AppKit
- NSApplication
-  modalWindow 

Instance Property

# modalWindow

The modal window displayed by the app.

macOS

``` source
@MainActor
var modalWindow: NSWindow? { get }
```

## Discussion

This property contains the current standalone modal window or `nil` if no modal window is being displayed. This property does not contain sheets that are attached to other windows. To retrieve a sheet, use the attachedSheet method of NSWindow.

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

func beginModalSession(for: NSWindow) -> NSApplication.ModalSession

Sets up a modal session with the given window and returns a pointer to the `NSModalSession` structure representing the session.

func runModalSession(NSApplication.ModalSession) -> NSApplication.ModalResponse

Runs a given modal session, as defined in a previous invocation of beginModalSession(for:).

struct ModalResponse

A set of button return values for modal dialogs.

typealias ModalSession

Variables of type `NSModalSession` point to information used by the system between `NSApplication`’s beginModalSession(for:) and endModalSession(_:) messages.

