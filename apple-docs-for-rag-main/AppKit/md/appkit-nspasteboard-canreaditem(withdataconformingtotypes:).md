

- AppKit
- NSPasteboard
-  canReadItem(withDataConformingToTypes:) 

Instance Method

# canReadItem(withDataConformingToTypes:)

Returns a Boolean value that indicates whether the receiver contains any items that conform to the specified UTIs.

macOS 10.6+

``` source
func canReadItem(withDataConformingToTypes types: [String]) -> Bool
```

## Parameters 

`types`  

An array of `NSString` objects containing UTIs.

## Return Value

true if the receiver contains any items that conform to the UTIs specified in `types`, otherwise false.

## See Also

### Related Documentation

func readObjects(forClasses: [AnyClass], options: [NSPasteboard.ReadingOptionKey : Any]?) -> [Any]?

Reads from the receiver objects that best match the specified array of classes.

### Validating Contents

func availableType(from: [NSPasteboard.PasteboardType]) -> NSPasteboard.PasteboardType?

Scans the specified types for a type that the receiver supports.

func canReadObject(forClasses: [AnyClass], options: [NSPasteboard.ReadingOptionKey : Any]?) -> Bool

Returns a Boolean value that indicates whether the receiver contains any items that can be represented as an instance of any class in a given array.

var types: [NSPasteboard.PasteboardType]?

An array of the receiver’s supported data types.

class func types(filterableTo: NSPasteboard.PasteboardType) -> [NSPasteboard.PasteboardType]

Returns the data types that can be converted to the specified type using the available filter services.

