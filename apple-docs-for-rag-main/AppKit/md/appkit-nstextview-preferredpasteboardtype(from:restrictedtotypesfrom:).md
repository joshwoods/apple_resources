

- AppKit
- NSTextView
-  preferredPasteboardType(from:restrictedToTypesFrom:) 

Instance Method

# preferredPasteboardType(from:restrictedToTypesFrom:)

Returns whatever type on the pasteboard would be most preferred for copying data.

macOS

``` source
@MainActor
func preferredPasteboardType(
    from availableTypes: [NSPasteboard.PasteboardType],
    restrictedToTypesFrom allowedTypes: [NSPasteboard.PasteboardType]?
) -> NSPasteboard.PasteboardType?
```

## Parameters 

`availableTypes`  

The types currently available on the pasteboard.

`allowedTypes`  

Types allowed in the return value. If `nil`, any available type is allowed.

## Return Value

The preferred type to provide given the available types and the allowed types.

## Discussion

You should not need to override this method. You should also not need to invoke it unless you are implementing a new type of pasteboard to handle services other than copy/paste or dragging.

## See Also

### Related Documentation

func pasteAsRichText(Any?)

This action method inserts the contents of the pasteboard into the receiver’s text as rich text, maintaining its attributes.

func pasteAsPlainText(Any?)

Inserts the contents of the pasteboard into the receiver’s text as plain text.

### Managing the pasteboard

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

func validRequestor(forSendType: NSPasteboard.PasteboardType?, returnType: NSPasteboard.PasteboardType?) -> Any?

Returns `self` if the text view can provide and accept the specified data types, or `nil` if it can’t.

