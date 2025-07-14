

- AppKit
- NSPasteboard
-  writeObjects(\_:) 

Instance Method

# writeObjects(\_:)

Writes an array of objects to the receiver.

macOS 10.6+

``` source
func writeObjects(_ objects: [any NSPasteboardWriting]) -> Bool
```

## Parameters 

`objects`  

An array of objects that implement the NSPasteboardWriting protocol (including instances of NSPasteboardItem).

## Return Value

true if the array was successfully added, otherwise false.

## See Also

### Writing Data

func clearContents() -> Int

Clears the existing contents of the pasteboard.

func setData(Data?, forType: NSPasteboard.PasteboardType) -> Bool

Sets the data as the representation for the specified type for the first item on the receiver.

func setPropertyList(Any, forType: NSPasteboard.PasteboardType) -> Bool

Sets the given property list as the representation for the specified type for the first item on the receiver.

func setString(String, forType: NSPasteboard.PasteboardType) -> Bool

Sets the given string as the representation for the specified type for the first item on the receiver.

struct PasteboardType

The supported pasteboard types.

