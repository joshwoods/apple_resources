

- AppKit
- NSPasteboard
-  types 

Instance Property

# types

An array of the receiver’s supported data types.

macOS

``` source
var types: [NSPasteboard.PasteboardType]? { get }
```

## Discussion

The types array is an array of NSString objects containing the union of the types of data declared for all the pasteboard items on the receiver. The returned types are listed in the order they were declared. It’s a good idea to check the value of types (or call availableType(from:)) before reading any data from an `NSPasteboard` object. If you need to see if a type in the types array matches a type string you have stored locally, use the isEqual(to:) method to perform the comparison.

## See Also

### Related Documentation

func declareTypes([NSPasteboard.PasteboardType], owner: Any?) -> Int

Prepares the receiver for a change in its contents by declaring the new types of data it will contain and a new owner.

func data(forType: NSPasteboard.PasteboardType) -> Data?

Returns the data for the specified type from the first item in the receiver that contains the type.

### Validating Contents

func availableType(from: [NSPasteboard.PasteboardType]) -> NSPasteboard.PasteboardType?

Scans the specified types for a type that the receiver supports.

func canReadItem(withDataConformingToTypes: [String]) -> Bool

Returns a Boolean value that indicates whether the receiver contains any items that conform to the specified UTIs.

func canReadObject(forClasses: [AnyClass], options: [NSPasteboard.ReadingOptionKey : Any]?) -> Bool

Returns a Boolean value that indicates whether the receiver contains any items that can be represented as an instance of any class in a given array.

class func types(filterableTo: NSPasteboard.PasteboardType) -> [NSPasteboard.PasteboardType]

Returns the data types that can be converted to the specified type using the available filter services.

