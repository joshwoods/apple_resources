

- AppKit
- NSPasteboardItem
-  types 

Instance Property

# types

An array of uniform type identifier strings of the data types that the receiver supports.

macOS 10.6+

``` source
var types: [NSPasteboard.PasteboardType] { get }
```

## See Also

### Getting types

func availableType(from: [NSPasteboard.PasteboardType]) -> NSPasteboard.PasteboardType?

Returns from a given array of types the first type within the pasteboard item, according to the ordering of types.

