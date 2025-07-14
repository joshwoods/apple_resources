

- AppKit
- NSApplication
-  endModalSession(\_:) 

Instance Method

# endModalSession(\_:)

Finishes a modal session.

macOS

``` source
@MainActor
func endModalSession(_ session: NSApplication.ModalSession)
```

## Parameters 

`session`  

A modal session structure returned by a previous invocation of beginModalSession(for:).

## See Also

### Related Documentation

func beginModalSession(for: NSWindow) -> NSApplication.ModalSession

Sets up a modal session with the given window and returns a pointer to the `NSModalSession` structure representing the session.

func runModalSession(NSApplication.ModalSession) -> NSApplication.ModalResponse

Runs a given modal session, as defined in a previous invocation of beginModalSession(for:).

### Methods

func activate(ignoringOtherApps: Bool)

Makes the receiver the active app.

Deprecated

func beginSheet(NSWindow, modalFor: NSWindow, modalDelegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer!)

Starts a document modal session.

Deprecated

func endSheet(NSWindow)

Ends a document modal session by specifying the sheet window.

Deprecated

func endSheet(NSWindow, returnCode: Int)

Ends a document modal session by specifying the sheet window.

Deprecated

