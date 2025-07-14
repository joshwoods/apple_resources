

- AppKit
- NSPasteboard
-  availableType(from:) 

Instance Method

# availableType(from:)

Scans the specified types for a type that the receiver supports.

macOS

``` source
func availableType(from types: [NSPasteboard.PasteboardType]) -> NSPasteboard.PasteboardType?
```

## Parameters 

`types`  

An array of `NSString` objects specifying the pasteboard types your application supports, in preferred order.

## Return Value

The first pasteboard type in `types` that is available on the pasteboard, or `nil` if the receiver does not contain any of the types in `types`.

## Discussion

You use this method to determine the best representation available on the pasteboard. For example, if your application supports RTFD, RTF, and string data, then you might invoke the method as follows:

```
NSArray *supportedTypes =
    [NSArray arrayWithObjects: NSRTFDPboardType, NSRTFPboardType, NSStringPboardType, nil];
NSString *bestType = [[NSPasteboard generalPasteboard]
    availableTypeFromArray:supportedTypes];
```

If the pasteboard contains RTF and string data, then `bestType` would contain `NSRTFPboardType`. If the pasteboard contains none of the types in `supportedTypes`, then `bestType` would be `nil`.

You must send a types or availableType(from:) message before reading any data from an `NSPasteboard` object. If you need to see if a type in the returned array matches a type string you have stored locally, use the isEqual(to:) method to perform the comparison.

## See Also

### Validating Contents

func canReadItem(withDataConformingToTypes: [String]) -> Bool

Returns a Boolean value that indicates whether the receiver contains any items that conform to the specified UTIs.

func canReadObject(forClasses: [AnyClass], options: [NSPasteboard.ReadingOptionKey : Any]?) -> Bool

Returns a Boolean value that indicates whether the receiver contains any items that can be represented as an instance of any class in a given array.

var types: [NSPasteboard.PasteboardType]?

An array of the receiver’s supported data types.

class func types(filterableTo: NSPasteboard.PasteboardType) -> [NSPasteboard.PasteboardType]

Returns the data types that can be converted to the specified type using the available filter services.

