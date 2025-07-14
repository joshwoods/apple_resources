

- AppKit
- NSPasteboard
-  canReadObject(forClasses:options:) 

Instance Method

# canReadObject(forClasses:options:)

Returns a Boolean value that indicates whether the receiver contains any items that can be represented as an instance of any class in a given array.

macOS 10.6+

``` source
func canReadObject(
    forClasses classArray: [AnyClass],
    options: [NSPasteboard.ReadingOptionKey : Any]? = nil
) -> Bool
```

## Parameters 

`classArray`  

An array of class objects.

Classes in the array must conform to the NSPasteboardReading protocol.

`options`  

A dictionary that specifies options to refine the search for pasteboard items, for example to restrict the search to file URLs with particular content types. For valid dictionary keys, see `Pasteboard Reading Options`.

## Return Value

true if the receiver contains any items that can be represented as an instance of a class specified in `classArray`, otherwise false.

## See Also

### Related Documentation

func readObjects(forClasses: [AnyClass], options: [NSPasteboard.ReadingOptionKey : Any]?) -> [Any]?

Reads from the receiver objects that best match the specified array of classes.

### Validating Contents

func availableType(from: [NSPasteboard.PasteboardType]) -> NSPasteboard.PasteboardType?

Scans the specified types for a type that the receiver supports.

func canReadItem(withDataConformingToTypes: [String]) -> Bool

Returns a Boolean value that indicates whether the receiver contains any items that conform to the specified UTIs.

var types: [NSPasteboard.PasteboardType]?

An array of the receiver’s supported data types.

class func types(filterableTo: NSPasteboard.PasteboardType) -> [NSPasteboard.PasteboardType]

Returns the data types that can be converted to the specified type using the available filter services.

