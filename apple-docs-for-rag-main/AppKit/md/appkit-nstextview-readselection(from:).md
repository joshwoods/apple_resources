

- AppKit
- NSTextView
-  readSelection(from:) 

Instance Method

# readSelection(from:)

Reads the text view’s preferred type of data from the specified pasteboard.

macOS

``` source
@MainActor
func readSelection(from pboard: NSPasteboard) -> Bool
```

## Parameters 

`pboard`  

The pasteboard to read from.

## Return Value

true if the data was successfully read, false otherwise.

## Discussion

This method invokes the preferredPasteboardType(from:restrictedToTypesFrom:) method to determine the text view’s preferred type of data and then reads the data using the readSelection(from:type:) method.

You should not need to override this method. You might need to invoke this method if you are implementing a new type of pasteboard to handle services other than copy/paste or dragging.

## See Also

### Managing the pasteboard

func preferredPasteboardType(from: [NSPasteboard.PasteboardType], restrictedToTypesFrom: [NSPasteboard.PasteboardType]?) -> NSPasteboard.PasteboardType?

Returns whatever type on the pasteboard would be most preferred for copying data.

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

func validRequestor(forSendType: NSPasteboard.PasteboardType?, returnType: NSPasteboard.PasteboardType?) -> Any?

Returns `self` if the text view can provide and accept the specified data types, or `nil` if it can’t.

