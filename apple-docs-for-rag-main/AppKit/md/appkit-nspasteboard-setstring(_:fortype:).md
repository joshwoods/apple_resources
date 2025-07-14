

- AppKit
- NSPasteboard
-  setString(\_:forType:) 

Instance Method

# setString(\_:forType:)

Sets the given string as the representation for the specified type for the first item on the receiver.

macOS

``` source
func setString(
    _ string: String,
    forType dataType: NSPasteboard.PasteboardType
) -> Bool
```

## Parameters 

`string`  

The string to write to the pasteboard.

`dataType`  

The type of string data. The type must have been declared by a previous declareTypes(_:owner:) message.

## Return Value

true if the data was written successfully, otherwise false if ownership of the pasteboard has changed. Any other error raises an `NSPasteboardCommunicationException`.

## Mentioned in 

Supporting Writing Tools via the pasteboard

## Discussion

This method invokes setData(_:forType:) to perform the write.

## See Also

### Related Documentation

func string(forType: NSPasteboard.PasteboardType) -> String?

Returns a concatenation of the strings for the specified type from all the items in the receiver that contain the type.

### Writing Data

func clearContents() -> Int

Clears the existing contents of the pasteboard.

func writeObjects([any NSPasteboardWriting]) -> Bool

Writes an array of objects to the receiver.

func setData(Data?, forType: NSPasteboard.PasteboardType) -> Bool

Sets the data as the representation for the specified type for the first item on the receiver.

func setPropertyList(Any, forType: NSPasteboard.PasteboardType) -> Bool

Sets the given property list as the representation for the specified type for the first item on the receiver.

struct PasteboardType

The supported pasteboard types.

