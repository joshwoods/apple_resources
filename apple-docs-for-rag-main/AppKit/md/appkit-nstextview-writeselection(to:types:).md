

- AppKit
- NSTextView
-  writeSelection(to:types:) 

Instance Method

# writeSelection(to:types:)

Writes the current selection to the specified pasteboard under each given type.

macOS

``` source
@MainActor
func writeSelection(
    to pboard: NSPasteboard,
    types: [NSPasteboard.PasteboardType]
) -> Bool
```

## Parameters 

`pboard`  

The pasteboard to write to.

`types`  

An array of strings describing the types of data to write.

## Return Value

true if the data for any single type was successfully written, false otherwise.

## Discussion

This method declares the data types on `pboard` and then invokes writeSelection(to:type:) or the delegate method textView(_:write:at:to:type:) for each type in the `types` array.

You should not need to override this method. You might need to invoke this method if you are implementing a new type of pasteboard to handle services other than copy/paste or dragging.

## See Also

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

func validRequestor(forSendType: NSPasteboard.PasteboardType?, returnType: NSPasteboard.PasteboardType?) -> Any?

Returns `self` if the text view can provide and accept the specified data types, or `nil` if it can’t.

