

- AppKit
- NSTextView
-  writeSelection(to:type:) 

Instance Method

# writeSelection(to:type:)

Writes the current selection to the specified pasteboard using the given type.

macOS

``` source
@MainActor
func writeSelection(
    to pboard: NSPasteboard,
    type: NSPasteboard.PasteboardType
) -> Bool
```

## Parameters 

`pboard`  

The pasteboard to write to.

`type`  

The type of data to write.

## Return Value

true if the data was successfully written, false otherwise.

## Discussion

The complete set of data types being written to `pboard` should be declared before invoking this method.

This method should be invoked only from writeSelection(to:types:). You can override this method to add support for writing new types of data to the pasteboard. You should invoke `super`’s implementation of the method to handle any types of data your overridden version does not.

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

func writeSelection(to: NSPasteboard, types: [NSPasteboard.PasteboardType]) -> Bool

Writes the current selection to the specified pasteboard under each given type.

func validRequestor(forSendType: NSPasteboard.PasteboardType?, returnType: NSPasteboard.PasteboardType?) -> Any?

Returns `self` if the text view can provide and accept the specified data types, or `nil` if it can’t.

