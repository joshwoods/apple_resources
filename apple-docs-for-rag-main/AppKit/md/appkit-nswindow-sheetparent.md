

- AppKit
- NSWindow
-  sheetParent 

Instance Property

# sheetParent

The window to which the sheet is attached.

macOS 10.9+

``` source
@MainActor
var sheetParent: NSWindow? { get }
```

## Discussion

The value of this property is `nil` if the receiver is not a sheet or has no sheet parent.

The window object in this property refers to the window to which the sheet is logically attached, regardless of appearance. The parent window–sheet relationship begins with the beginning of the sheet (for example, through beginSheet(_:completionHandler:)) and ends with the sheet’s dismissal (for example, through endSheet(_:)).

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

var sheets: [NSWindow]

An array of the sheets currently attached to the window.

