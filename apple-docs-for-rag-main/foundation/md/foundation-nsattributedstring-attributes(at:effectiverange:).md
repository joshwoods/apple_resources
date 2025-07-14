

- Foundation
- NSAttributedString
-  attributes(at:effectiveRange:) 

Instance Method

# attributes(at:effectiveRange:)

Returns the attributes for the character at the specified index.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func attributes(
    at location: Int,
    effectiveRange range: NSRangePointer?
) -> [NSAttributedString.Key : Any]
```

## Parameters 

`location`  

The index for which to return attributes. This value must lie within the bounds of the receiver.

`range`  

Upon return, the range over which the attributes and values are the same as those at `index`. This range isn’t necessarily the maximum range covered, and its extent is implementation-dependent. If you need the maximum range, use attributes(at:longestEffectiveRange:in:). If you don’t need this value, pass `NULL`.

## Return Value

The attributes for the character at `index`.

## Discussion

Raises an rangeException if `index` lies beyond the end of the receiver’s characters.

For a list of possible attributes, see NSAttributedString.Key.

## See Also

### Getting attributes for a range of text

func attributes(at: Int, longestEffectiveRange: NSRangePointer?, in: NSRange) -> [NSAttributedString.Key : Any]

Returns the attributes for the character at the specified index and, by reference, the range where the attributes apply.

func attribute(NSAttributedString.Key, at: Int, effectiveRange: NSRangePointer?) -> Any?

Returns the value for an attribute with the specified name of the character at the specified index and, by reference, the range where the attribute applies.

func attribute(NSAttributedString.Key, at: Int, longestEffectiveRange: NSRangePointer?, in: NSRange) -> Any?

Returns the value for the attribute with the specified name of the character at the specified index and, by reference, the range where the attribute applies.

func enumerateAttribute(NSAttributedString.Key, in: NSRange, options: NSAttributedString.EnumerationOptions, using: (Any?, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes the specified closure or block for each range of a particular attribute in the attributed string.

func enumerateAttributes(in: NSRange, options: NSAttributedString.EnumerationOptions, using: ([NSAttributedString.Key : Any], NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes the specified closure or block for each range of attributes in the attributed string.

struct EnumerationOptions

Options for enumerating attributes.

