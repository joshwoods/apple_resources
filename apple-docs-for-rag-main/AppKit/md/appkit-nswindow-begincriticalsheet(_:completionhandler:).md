

- AppKit
- NSWindow
-  beginCriticalSheet(\_:completionHandler:) 

Instance Method

# beginCriticalSheet(\_:completionHandler:)

Starts a document-modal session and presents the specified critical sheet.

macOS 10.9+

``` source
@MainActor
func beginCriticalSheet(
    _ sheetWindow: NSWindow,
    completionHandler handler: ((NSApplication.ModalResponse) -> Void)? = nil
)
```

``` source
@MainActor
func beginCriticalSheet(_ sheetWindow: NSWindow) async -> NSApplication.ModalResponse
```

## Parameters 

`sheetWindow`  

The window object that represents the critical sheet to present. A critical sheet contains content that is time-critical or very important to the user.

`handler`  

The completion handler that gets called when the sheet’s modal session ends.

## Discussion

This method displays the sheet—on top of the window’s current sheet, if one exists—makes it key and returns control to the caller. While the sheet remains visible, most events targeted at the receiver are prohibited. The runloop does not enter any special mode to accomplish this.

If the window already has a sheet when this method runs, the existing sheet is temporarily disabled while the critical sheet is presented. When the critical sheet is dismissed, the previously presented sheet continues its standard operation.

## See Also

### Managing Sheets

var attachedSheet: NSWindow?

The sheet attached to the window.

var isSheet: Bool

A Boolean value that indicates whether the window has ever run as a modal sheet.

func beginSheet(NSWindow, completionHandler: ((NSApplication.ModalResponse) -> Void)?)

Starts a document-modal session and presents—or queues for presentation—a sheet.

func endSheet(NSWindow)

Ends a document-modal session and dismisses the specified sheet.

func endSheet(NSWindow, returnCode: NSApplication.ModalResponse)

Ends a document-modal session and dismisses the specified sheet.

var sheetParent: NSWindow?

The window to which the sheet is attached.

var sheets: [NSWindow]

An array of the sheets currently attached to the window.

