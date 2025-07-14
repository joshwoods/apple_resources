

- AppKit
- NSPasteboardItem
-  availableType(from:) 

Instance Method

# availableType(from:)

Returns from a given array of types the first type within the pasteboard item, according to the ordering of types.

macOS 10.6+

``` source
func availableType(from types: [NSPasteboard.PasteboardType]) -> NSPasteboard.PasteboardType?
```

## Parameters 

`types`  

An array of strings representing UTIs, arranged in order of preference (most preferred as the 0th element in the array).

## Return Value

The first (according to the sender’s ordering of `types`) type in `types` contained in the pasteboard item, or `nil` if the receiver does not contain any types given in `types`.

## Discussion

The method checks for UTI conformance of the requested types, preferring an exact match to conformance.

## See Also

### Getting types

var types: [NSPasteboard.PasteboardType]

An array of uniform type identifier strings of the data types that the receiver supports.

