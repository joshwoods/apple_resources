

- AppKit
- NSApplication
-  endSheet(\_:) Deprecated

Instance Method

# endSheet(\_:)

Ends a document modal session by specifying the sheet window.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func endSheet(_ sheet: NSWindow)
```

Deprecated

Use endSheet(_:) method of NSWindow instead.

## Parameters 

`sheet`  

The sheet whose modal session you want to end.

## Discussion

This method ends the modal session with the return code stop.

## See Also

### Methods

func activate(ignoringOtherApps: Bool)

Makes the receiver the active app.

Deprecated

func endModalSession(NSApplication.ModalSession)

Finishes a modal session.

func beginSheet(NSWindow, modalFor: NSWindow, modalDelegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer!)

Starts a document modal session.

Deprecated

func endSheet(NSWindow, returnCode: Int)

Ends a document modal session by specifying the sheet window.

Deprecated

