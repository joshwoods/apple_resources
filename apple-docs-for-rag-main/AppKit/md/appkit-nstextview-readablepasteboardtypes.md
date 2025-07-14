

- AppKit
- NSTextView
-  readablePasteboardTypes 

Instance Property

# readablePasteboardTypes

The types this text view can read immediately from the pasteboard.

macOS

``` source
@MainActor
var readablePasteboardTypes: [NSPasteboard.PasteboardType] { get }
```

## See Also

### Managing the pasteboard

func preferredPasteboardType(from: [NSPasteboard.PasteboardType], restrictedToTypesFrom: [NSPasteboard.PasteboardType]?) -> NSPasteboard.PasteboardType?

Returns whatever type on the pasteboard would be most preferred for copying data.

func readSelection(from: NSPasteboard) -> Bool

Reads the text view’s preferred type of data from the specified pasteboard.

func readSelection(from: NSPasteboard, type: NSPasteboard.PasteboardType) -> Bool

Reads data of the given type from the specified pasteboard.

var writablePasteboardTypes: [NSPasteboard.PasteboardType]

The pasteboard types that can be provided from the current selection.

func writeSelection(to: NSPasteboard, type: NSPasteboard.PasteboardType) -> Bool

Writes the current selection to the specified pasteboard using the given type.

func writeSelection(to: NSPasteboard, types: [NSPasteboard.PasteboardType]) -> Bool

Writes the current selection to the specified pasteboard under each given type.

func validRequestor(forSendType: NSPasteboard.PasteboardType?, returnType: NSPasteboard.PasteboardType?) -> Any?

Returns `self` if the text view can provide and accept the specified data types, or `nil` if it can’t.

