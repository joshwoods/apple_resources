

- AppKit
- NSPasteboard
-  setPropertyList(\_:forType:) 

Instance Method

# setPropertyList(\_:forType:)

Sets the given property list as the representation for the specified type for the first item on the receiver.

macOS

``` source
func setPropertyList(
    _ plist: Any,
    forType dataType: NSPasteboard.PasteboardType
) -> Bool
```

## Parameters 

`plist`  

The property list data to write to the pasteboard.

`dataType`  

The type of property-list data in the `propertyList` parameter. The type must have been declared by a previous declareTypes(_:owner:) message.

## Return Value

true if the data was written successfully, otherwise false if ownership of the pasteboard has changed. Any other error raises an `NSPasteboardCommunicationException`.

## Discussion

This method invokes setData(_:forType:) with a serialized property list parameter.

## See Also

### Related Documentation

func propertyList(forType: NSPasteboard.PasteboardType) -> Any?

Returns the property list for the specified type from the first item in the receiver that contains the type.

### Writing Data

func clearContents() -> Int

Clears the existing contents of the pasteboard.

func writeObjects([any NSPasteboardWriting]) -> Bool

Writes an array of objects to the receiver.

func setData(Data?, forType: NSPasteboard.PasteboardType) -> Bool

Sets the data as the representation for the specified type for the first item on the receiver.

func setString(String, forType: NSPasteboard.PasteboardType) -> Bool

Sets the given string as the representation for the specified type for the first item on the receiver.

struct PasteboardType

The supported pasteboard types.

