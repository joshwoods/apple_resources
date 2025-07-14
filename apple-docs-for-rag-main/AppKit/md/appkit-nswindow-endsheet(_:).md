

- AppKit
- NSWindow
-  endSheet(\_:) 

Instance Method

# endSheet(\_:)

Ends a document-modal session and dismisses the specified sheet.

macOS 10.9+

``` source
@MainActor
func endSheet(_ sheetWindow: NSWindow)
```

## Parameters 

`sheetWindow`  

The window object that represents the sheet to be dismissed.

## Discussion

This method ends the modal session with the return code `NSModalResponseStop`.

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

func endSheet(NSWindow, returnCode: NSApplication.ModalResponse)

Ends a document-modal session and dismisses the specified sheet.

var sheetParent: NSWindow?

The window to which the sheet is attached.

var sheets: [NSWindow]

An array of the sheets currently attached to the window.

