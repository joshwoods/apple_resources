

- AppKit
- NSWindow
-  sheets 

Instance Property

# sheets

An array of the sheets currently attached to the window.

macOS 10.9+

``` source
@MainActor
var sheets: [NSWindow] { get }
```

## Discussion

The value of this property is an ordered array that contains—in top-to-bottom order—the presented sheets that are attached to the window, followed by queued sheets, in the order they were queued. The array doesn’t include nested sheets or subsheets.

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

func endSheet(NSWindow, returnCode: NSApplication.ModalResponse)

Ends a document-modal session and dismisses the specified sheet.

var sheetParent: NSWindow?

The window to which the sheet is attached.

