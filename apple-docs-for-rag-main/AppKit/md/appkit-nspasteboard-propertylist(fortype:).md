

- AppKit
- NSPasteboard
-  propertyList(forType:) 

Instance Method

# propertyList(forType:)

Returns the property list for the specified type from the first item in the receiver that contains the type.

macOS

``` source
func propertyList(forType dataType: NSPasteboard.PasteboardType) -> Any?
```

## Parameters 

`dataType`  

The pasteboard data type containing the property-list data.

## Return Value

A property list of objects of the specified type, obtained from the first item in the receiver that contains the type. The returned property list can contain any combination of objects, as long as each object is a valid property-list type (for a list of types, see Property list).

## Discussion

This method invokes the data(forType:) method.

### Special Considerations

It’s a good idea to check types or call availableType(from:) before invoking propertyList(forType:). Although performing this check isn’t required, doing so can help you determine if a `nil` result from a reading method is due to something like a pasteboard timeout.

## See Also

### Related Documentation

func setPropertyList(Any, forType: NSPasteboard.PasteboardType) -> Bool

Sets the given property list as the representation for the specified type for the first item on the receiver.

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

func string(forType: NSPasteboard.PasteboardType) -> String?

Returns a concatenation of the strings for the specified type from all the items in the receiver that contain the type.

