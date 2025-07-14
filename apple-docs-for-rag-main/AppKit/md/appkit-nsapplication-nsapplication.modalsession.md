

- AppKit
- NSApplication
-  NSApplication.ModalSession 

Type Alias

# NSApplication.ModalSession

Variables of type `NSModalSession` point to information used by the system between `NSApplication`’s beginModalSession(for:) and endModalSession(_:) messages.

macOS

``` source
typealias ModalSession = OpaquePointer
```

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

var modalWindow: NSWindow?

The modal window displayed by the app.

struct ModalResponse

A set of button return values for modal dialogs.

