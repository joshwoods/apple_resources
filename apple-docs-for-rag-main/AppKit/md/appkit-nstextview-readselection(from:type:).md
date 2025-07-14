

- AppKit
- NSTextView
-  readSelection(from:type:) 

Instance Method

# readSelection(from:type:)

Reads data of the given type from the specified pasteboard.

macOS

``` source
@MainActor
func readSelection(
    from pboard: NSPasteboard,
    type: NSPasteboard.PasteboardType
) -> Bool
```

## Parameters 

`pboard`  

The pasteboard to read from.

`type`  

The type of data to read.

## Return Value

true if the data was successfully read, false otherwise.

## Discussion

The new data is placed at the current insertion point, replacing the current selection if one exists.

You should override this method to read pasteboard types other than the default types. Use the rangeForUserTextChange method to obtain the range of characters (if any) to be replaced by the new data.

## See Also

### Related Documentation

var rangeForUserTextChange: NSRange

The range of characters affected by a method that changes characters (as opposed to attributes).

### Managing the pasteboard

func preferredPasteboardType(from: [NSPasteboard.PasteboardType], restrictedToTypesFrom: [NSPasteboard.PasteboardType]?) -> NSPasteboard.PasteboardType?

Returns whatever type on the pasteboard would be most preferred for copying data.

func readSelection(from: NSPasteboard) -> Bool

Reads the text view’s preferred type of data from the specified pasteboard.

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

