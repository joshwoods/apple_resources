

- AppKit
- NSPasteboard
-  setData(\_:forType:) 

Instance Method

# setData(\_:forType:)

Sets the data as the representation for the specified type for the first item on the receiver.

macOS

``` source
func setData(
    _ data: Data?,
    forType dataType: NSPasteboard.PasteboardType
) -> Bool
```

## Parameters 

`data`  

The data to write to the pasteboard.

`dataType`  

The type of data in the `data` parameter. The type must have been declared by a previous declareTypes(_:owner:) message.

## Return Value

true if the data was written successfully, otherwise false if ownership of the pasteboard has changed. Any other error raises an `NSPasteboardCommunicationException`.

## See Also

### Related Documentation

func data(forType: NSPasteboard.PasteboardType) -> Data?

Returns the data for the specified type from the first item in the receiver that contains the type.

### Writing Data

func clearContents() -> Int

Clears the existing contents of the pasteboard.

func writeObjects([any NSPasteboardWriting]) -> Bool

Writes an array of objects to the receiver.

func setPropertyList(Any, forType: NSPasteboard.PasteboardType) -> Bool

Sets the given property list as the representation for the specified type for the first item on the receiver.

func setString(String, forType: NSPasteboard.PasteboardType) -> Bool

Sets the given string as the representation for the specified type for the first item on the receiver.

struct PasteboardType

The supported pasteboard types.

