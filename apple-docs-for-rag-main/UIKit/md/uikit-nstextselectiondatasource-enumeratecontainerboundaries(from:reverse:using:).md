

- UIKit
- NSTextSelectionDataSource
-  enumerateContainerBoundaries(from:reverse:using:) 

Instance Method

# enumerateContainerBoundaries(from:reverse:using:)

Enumerates all the container boundaries starting from the location you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
optional func enumerateContainerBoundaries(
    from location: any NSTextLocation,
    reverse: Bool,
    using block: (any NSTextLocation, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`location`  

The location where the enumeration starts.

`reverse`  

A Boolean value that indicates the enumeration starts at the end of the container.

`block`  

AA closure to invoke to evaluate the container boundaries; end the enumeration early by returning `false`.

## Discussion

This is an optional method you implement to enumerate the text up to the container or page boundary when the text selection data provider supports this layout functionality.

## See Also

### Enumerating components of the selection

func enumerateCaretOffsetsInLineFragment(at: any NSTextLocation, using: (CGFloat, any NSTextLocation, Bool, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the insertion point caret offsets from left to right in visual order.

**Required**

func enumerateSubstrings(from: any NSTextLocation, options: NSString.EnumerationOptions, using: (String?, NSTextRange, NSTextRange?, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates the textual segment boundaries starting at the location you specify.

**Required**

