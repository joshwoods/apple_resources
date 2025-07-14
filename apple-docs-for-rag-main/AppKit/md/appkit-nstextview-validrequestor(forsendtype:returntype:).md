

- AppKit
- NSTextView
-  validRequestor(forSendType:returnType:) 

Instance Method

# validRequestor(forSendType:returnType:)

Returns `self` if the text view can provide and accept the specified data types, or `nil` if it can’t.

macOS

``` source
@MainActor
func validRequestor(
    forSendType sendType: NSPasteboard.PasteboardType?,
    returnType: NSPasteboard.PasteboardType?
) -> Any?
```

## Parameters 

`sendType`  

The type of data requested.

`returnType`  

The type of data that will be returned.

## Return Value

`self` if `sendType` specifies a type of data the text view can put on the pasteboard and `returnType` contains a type of data the text view can read from the pasteboard; otherwise `nil`.

## See Also

### Related Documentation

func validRequestor(forSendType: NSPasteboard.PasteboardType?, returnType: NSPasteboard.PasteboardType?) -> Any?

Overridden by subclasses to determine what services are available.

### Managing the pasteboard

func preferredPasteboardType(from: [NSPasteboard.PasteboardType], restrictedToTypesFrom: [NSPasteboard.PasteboardType]?) -> NSPasteboard.PasteboardType?

Returns whatever type on the pasteboard would be most preferred for copying data.

func readSelection(from: NSPasteboard) -> Bool

Reads the text view’s preferred type of data from the specified pasteboard.

func readSelection(from: NSPasteboard, type: NSPasteboard.PasteboardType) -> Bool

Reads data of the given type from the specified pasteboard.

var readablePasteboardTypes: [NSPasteboard.PasteboardType]

The types this text view can read immediately from the pasteboard.

var writablePasteboardTypes: [NSPasteboard.PasteboardType]

The pasteboard types that can be provided from the current selection.

func writeSelection(to: NSPasteboard, type: NSPasteboard.PasteboardType) -> Bool

Writes the current selection to the specified pasteboard using the given type.

func writeSelection(to: NSPasteboard, types: [NSPasteboard.PasteboardType]) -> Bool

Writes the current selection to the specified pasteboard under each given type.

