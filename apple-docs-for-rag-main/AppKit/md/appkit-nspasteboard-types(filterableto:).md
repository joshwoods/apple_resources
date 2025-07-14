

- AppKit
- NSPasteboard
-  types(filterableTo:) 

Type Method

# types(filterableTo:)

Returns the data types that can be converted to the specified type using the available filter services.

macOS

``` source
class func types(filterableTo type: NSPasteboard.PasteboardType) -> [NSPasteboard.PasteboardType]
```

## Parameters 

`type`  

The target data type.

## Return Value

An array of `NSString` objects containing the types that can be converted to the target data type.

## Discussion

The array also contains the original type.

## See Also

### Validating Contents

func availableType(from: [NSPasteboard.PasteboardType]) -> NSPasteboard.PasteboardType?

Scans the specified types for a type that the receiver supports.

func canReadItem(withDataConformingToTypes: [String]) -> Bool

Returns a Boolean value that indicates whether the receiver contains any items that conform to the specified UTIs.

func canReadObject(forClasses: [AnyClass], options: [NSPasteboard.ReadingOptionKey : Any]?) -> Bool

Returns a Boolean value that indicates whether the receiver contains any items that can be represented as an instance of any class in a given array.

var types: [NSPasteboard.PasteboardType]?

An array of the receiver’s supported data types.

