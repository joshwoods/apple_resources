

- AppKit
- NSPasteboard
-  clearContents() 

Instance Method

# clearContents()

Clears the existing contents of the pasteboard.

macOS 10.6+

``` source
func clearContents() -> Int
```

## Return Value

The change count of the receiver.

## Discussion

Clears the existing contents of the pasteboard, preparing it for new contents. This is the first step in providing data on the pasteboard.

## See Also

### Writing Data

func writeObjects([any NSPasteboardWriting]) -> Bool

Writes an array of objects to the receiver.

func setData(Data?, forType: NSPasteboard.PasteboardType) -> Bool

Sets the data as the representation for the specified type for the first item on the receiver.

func setPropertyList(Any, forType: NSPasteboard.PasteboardType) -> Bool

Sets the given property list as the representation for the specified type for the first item on the receiver.

func setString(String, forType: NSPasteboard.PasteboardType) -> Bool

Sets the given string as the representation for the specified type for the first item on the receiver.

struct PasteboardType

The supported pasteboard types.

