

- AppKit
- NSTextSelectionDataSource
-  enumerateSubstrings(from:options:using:) 

Instance Method

# enumerateSubstrings(from:options:using:)

Enumerates the textual segment boundaries starting at the location you specify.

macOS 12.0+

``` source
func enumerateSubstrings(
    from location: any NSTextLocation,
    options: NSString.EnumerationOptions = [],
    using block: (String?, NSTextRange, NSTextRange?, UnsafeMutablePointer) -> Void
)
```

**Required**

## Parameters 

`location`  

The location where the enumeration starts.

`options`  

One or more of the available NSString.EnumerationOptions.

`block`  

A closure to invoke to evaluate the substrings; end the enumeration early by returning `false`.

## Discussion

## See Also

### Enumerating components of the selection

func enumerateCaretOffsetsInLineFragment(at: any NSTextLocation, using: (CGFloat, any NSTextLocation, Bool, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the insertion point caret offsets from left to right in visual order.

**Required**

func enumerateContainerBoundaries(from: any NSTextLocation, reverse: Bool, using: (any NSTextLocation, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the container boundaries starting from the location you specify.

