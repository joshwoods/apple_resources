

- AppKit
- NSTextSelectionDataSource
-  enumerateCaretOffsetsInLineFragment(at:using:) 

Instance Method

# enumerateCaretOffsetsInLineFragment(at:using:)

Enumerates all the insertion point caret offsets from left to right in visual order.

macOS 12.0+

``` source
func enumerateCaretOffsetsInLineFragment(
    at location: any NSTextLocation,
    using block: (CGFloat, any NSTextLocation, Bool, UnsafeMutablePointer) -> Void
)
```

**Required**

## Parameters 

`location`  

The `NSTextLocation` to start from.

`block`  

The closure to invoke once for each logical caret edge in the line fragment, in left-to-right visual order. End the enumeration early by returning `false`.

## Discussion

The `caretOffset` is in the coordinate system for the text container. When `leadingEdge` is `true`, it indicates that `caretOffset` is at the logical edge preceding the character. For left-to-right characters, the caret is on the left, and on the right for right-to-left characters.

## See Also

### Enumerating components of the selection

func enumerateContainerBoundaries(from: any NSTextLocation, reverse: Bool, using: (any NSTextLocation, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the container boundaries starting from the location you specify.

func enumerateSubstrings(from: any NSTextLocation, options: NSString.EnumerationOptions, using: (String?, NSTextRange, NSTextRange?, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates the textual segment boundaries starting at the location you specify.

**Required**

