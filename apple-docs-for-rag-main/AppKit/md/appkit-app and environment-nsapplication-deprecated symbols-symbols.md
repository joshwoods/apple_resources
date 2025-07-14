

- AppKit
- App and Environment
- NSApplication
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review symbols that are no longer supported, and find the replacements to use instead.

## Topics

### Methods

func activate(ignoringOtherApps: Bool)

Makes the receiver the active app.

Deprecated

func endModalSession(NSApplication.ModalSession)

Finishes a modal session.

func beginSheet(NSWindow, modalFor: NSWindow, modalDelegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer!)

Starts a document modal session.

Deprecated

func endSheet(NSWindow)

Ends a document modal session by specifying the sheet window.

Deprecated

func endSheet(NSWindow, returnCode: Int)

Ends a document modal session by specifying the sheet window.

Deprecated

