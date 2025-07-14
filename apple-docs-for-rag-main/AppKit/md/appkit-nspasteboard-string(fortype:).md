

- AppKit
- NSPasteboard
-  string(forType:) 

Instance Method

# string(forType:)

Returns a concatenation of the strings for the specified type from all the items in the receiver that contain the type.

macOS

``` source
func string(forType dataType: NSPasteboard.PasteboardType) -> String?
```

## Parameters 

`dataType`  

The pasteboard data type to read.

## Return Value

A concatenation of the strings for the specified type from all the items in the receiver that contain the type, or `nil` if none of the items contain strings of the specified type.

## Discussion

This method invokes data(forType:) to obtain the string. If the string cannot be obtained, string(forType:) returns `nil`. See data(forType:) for a description of what will cause `nil` to be returned.

In macOS 10.6 and later, if the receiver contains multiple items that can provide string, RTF, or RTFD data, the text data from each item is returned as a combined result separated by newlines.

### Special Considerations

It’s a good idea to check types or call availableType(from:) before invoking string(forType:). Although performing this check isn’t required, doing so can help you determine if a `nil` result from a reading method is due to something like a pasteboard timeout.

## See Also

### Related Documentation

func setString(String, forType: NSPasteboard.PasteboardType) -> Bool

Sets the given string as the representation for the specified type for the first item on the receiver.

### Reading Data

func readObjects(forClasses: [AnyClass], options: [NSPasteboard.ReadingOptionKey : Any]?) -> [Any]?

Reads from the receiver objects that best match the specified array of classes.

struct ReadingOptionKey

Options for reading pasteboard data.

struct ReadingOptions

Options that specify how to interpret data on the pasteboard when initializing pasteboard data.

var pasteboardItems: [NSPasteboardItem]?

An array that contains all the items held by the pasteboard.

func index(of: NSPasteboardItem) -> Int

Returns the index of the specified pasteboard item.

func data(forType: NSPasteboard.PasteboardType) -> Data?

Returns the data for the specified type from the first item in the receiver that contains the type.

func propertyList(forType: NSPasteboard.PasteboardType) -> Any?

Returns the property list for the specified type from the first item in the receiver that contains the type.

