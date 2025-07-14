

- AppKit
- NSApplication
-  beginSheet(\_:modalFor:modalDelegate:didEnd:contextInfo:) Deprecated

Instance Method

# beginSheet(\_:modalFor:modalDelegate:didEnd:contextInfo:)

Starts a document modal session.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func beginSheet(
    _ sheet: NSWindow,
    modalFor docWindow: NSWindow,
    modalDelegate: Any?,
    didEnd didEndSelector: Selector?,
    contextInfo: UnsafeMutableRawPointer!
)
```

Deprecated

Use the beginSheet(_:completionHandler:) method of NSWindow instead.

## Parameters 

`sheet`  

The window object representing the sheet you want to display.

`docWindow`  

The window object to which you want to attach the sheet.

`modalDelegate`  

The delegate object that defines your `didEndSelector` method. If `nil`, the method in `didEndSelector` is not called.

`didEndSelector`  

An optional method to call when the sheet’s modal session has ended. This method must be defined on the object in the `modalDelegate` parameter and have the following signature:

```
- (void)sheetDidEnd:(NSWindow *)sheet returnCode:(NSInteger)returnCode contextInfo:(void *)contextInfo;
```

`contextInfo`  

A pointer to the context info you want passed to the `didEndSelector` method when the sheet’s modal session ends.

## Discussion

This method displays the sheet modally on the specified window and returns control to the caller. Most events targeted at `docWindow` are prohibited while the sheet is displayed but the app’s main run loop runs normally otherwise.

## See Also

### Methods

func activate(ignoringOtherApps: Bool)

Makes the receiver the active app.

Deprecated

func endModalSession(NSApplication.ModalSession)

Finishes a modal session.

func endSheet(NSWindow)

Ends a document modal session by specifying the sheet window.

Deprecated

func endSheet(NSWindow, returnCode: Int)

Ends a document modal session by specifying the sheet window.

Deprecated

