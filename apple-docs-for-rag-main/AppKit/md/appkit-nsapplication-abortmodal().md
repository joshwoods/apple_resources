

- AppKit
- NSApplication
-  abortModal() 

Instance Method

# abortModal()

Aborts the event loop started by runModal(for:) or runModalSession(_:).

macOS

``` source
@MainActor
func abortModal()
```

## Discussion

When stopped with this method, runModal(for:) and runModalSession(_:) return `NSModalResponseAbort`.

abortModal() must be used instead of stopModal() or stopModal(withCode:) when you need to stop a modal event loop from anywhere other than a callout from that event loop. In other words, if you want to stop the loop in response to a user’s actions within the modal window, use stopModal(); otherwise, use abortModal(). For example, use abortModal() when running in a different thread from AppKit’s main thread or when responding to an `NSTimer` that you have added to the `NSModalPanelRunLoopMode` mode of the default `NSRunLoop`.

## See Also

### Related Documentation

func endModalSession(NSApplication.ModalSession)

Finishes a modal session.

### Running a Modal Window

func runModal(for: NSWindow) -> NSApplication.ModalResponse

Starts a modal event loop for the specified window.

func stopModal()

Stops a modal event loop.

func stopModal(withCode: NSApplication.ModalResponse)

Stops a modal event loop, allowing you to return a custom result code.

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

