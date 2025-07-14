

- AppKit
- NSApplication
-  endSheet(\_:returnCode:) Deprecated

Instance Method

# endSheet(\_:returnCode:)

Ends a document modal session by specifying the sheet window.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func endSheet(
    _ sheet: NSWindow,
    returnCode: Int
)
```

Deprecated

Use endSheet(_:returnCode:) method of NSWindow instead.

## Parameters 

`sheet`  

The sheet whose modal session you want to end.

`returnCode`  

The return code to send to the delegate. You can use one of the return codes defined in NSApplication.ModalResponse or a custom value that you define.

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

func endSheet(NSWindow)

Ends a document modal session by specifying the sheet window.

Deprecated

