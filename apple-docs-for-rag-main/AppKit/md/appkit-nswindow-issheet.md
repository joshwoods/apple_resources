

- AppKit
- NSWindow
-  isSheet 

Instance Property

# isSheet

A Boolean value that indicates whether the window has ever run as a modal sheet.

macOS

``` source
@MainActor
var isSheet: Bool { get }
```

## Discussion

The value of this property is true if the window has ever run as a modal sheet; otherwise, false.

## See Also

### Managing Sheets

var attachedSheet: NSWindow?

The sheet attached to the window.

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

var sheets: [NSWindow]

An array of the sheets currently attached to the window.

