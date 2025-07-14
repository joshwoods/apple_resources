

- AppKit
- NSWindow
-  endSheet(\_:returnCode:) 

Instance Method

# endSheet(\_:returnCode:)

Ends a document-modal session and dismisses the specified sheet.

macOS 10.9+

``` source
@MainActor
func endSheet(
    _ sheetWindow: NSWindow,
    returnCode: NSApplication.ModalResponse
)
```

## Parameters 

`sheetWindow`  

The window object that represents the sheet to dismiss.

`returnCode`  

The return code to send to the completion handler. You can use a custom value that you define or one of the return codes defined in the NSApplication.ModalResponse enumeration or `Additional NSModalResponse Values`.

## Discussion

This method ends the modal session with the specified return code.

## See Also

### Managing Sheets

var attachedSheet: NSWindow?

The sheet attached to the window.

var isSheet: Bool

A Boolean value that indicates whether the window has ever run as a modal sheet.

func beginSheet(NSWindow, completionHandler: ((NSApplication.ModalResponse) -> Void)?)

Starts a document-modal session and presents—or queues for presentation—a sheet.

func beginCriticalSheet(NSWindow, completionHandler: ((NSApplication.ModalResponse) -> Void)?)

Starts a document-modal session and presents the specified critical sheet.

func endSheet(NSWindow)

Ends a document-modal session and dismisses the specified sheet.

var sheetParent: NSWindow?

The window to which the sheet is attached.

var sheets: [NSWindow]

An array of the sheets currently attached to the window.

