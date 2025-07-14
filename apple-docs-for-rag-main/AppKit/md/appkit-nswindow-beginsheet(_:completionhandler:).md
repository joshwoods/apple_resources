

- AppKit
- NSWindow
-  beginSheet(\_:completionHandler:) 

Instance Method

# beginSheet(\_:completionHandler:)

Starts a document-modal session and presents—or queues for presentation—a sheet.

macOS 10.9+

``` source
@MainActor
func beginSheet(
    _ sheetWindow: NSWindow,
    completionHandler handler: ((NSApplication.ModalResponse) -> Void)? = nil
)
```

``` source
@MainActor
func beginSheet(_ sheetWindow: NSWindow) async -> NSApplication.ModalResponse
```

## Parameters 

`sheetWindow`  

The window object that represents the sheet to present.

`handler`  

The completion handler that gets called when the sheet’s modal session ends.

## Discussion

If the window already has a presented sheet, this method queues the specified sheet for presentation after the current sheet is dismissed and then returns control to the caller.

If the window has no presented sheets, this method displays the specified sheet, makes it key, and returns control to the caller. While the sheet remains visible, most events targeted at the receiver are prohibited. The runloop does not enter any special mode to accomplish this.

## See Also

### Managing Sheets

var attachedSheet: NSWindow?

The sheet attached to the window.

var isSheet: Bool

A Boolean value that indicates whether the window has ever run as a modal sheet.

func beginCriticalSheet(NSWindow, completionHandler: ((NSApplication.ModalResponse) -> Void)?)

Starts a document-modal session and presents the specified critical sheet.

func endSheet(NSWindow)

Ends a document-modal session and dismisses the specified sheet.

func endSheet(NSWindow, returnCode: NSApplication.ModalResponse)

Ends a document-modal session and dismisses the specified sheet.

var sheetParent: NSWindow?

The window to which the sheet is attached.

var sheets: [NSWindow]

An array of the sheets currently attached to the window.

