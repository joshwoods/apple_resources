

- Foundation
- NSAttributedString
-  attributes(at:longestEffectiveRange:in:) 

Instance Method

# attributes(at:longestEffectiveRange:in:)

Returns the attributes for the character at the specified index and, by reference, the range where the attributes apply.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func attributes(
    at location: Int,
    longestEffectiveRange range: NSRangePointer?,
    in rangeLimit: NSRange
) -> [NSAttributedString.Key : Any]
```

## Parameters 

`location`  

The index for which to return attributes. This value must not exceed the bounds of the receiver.

`range`  

If non-`NULL`, upon return contains the maximum range over which the attributes and values are the same as those at `index`, clipped to `rangeLimit`.

`rangeLimit`  

The range over which to search for continuous presence of the attributes at `index`. This value must not exceed the bounds of the receiver.

## Discussion

Raises an rangeException if `index` or any part of `rangeLimit` lies beyond the end of the receiver’s characters.

If you don’t need the range information, it’s far more efficient to use the attributes(at:effectiveRange:) method to retrieve the attribute value.

For a list of possible attributes, see NSAttributedString.Key.

## See Also

### Getting attributes for a range of text

func attributes(at: Int, effectiveRange: NSRangePointer?) -> [NSAttributedString.Key : Any]

Returns the attributes for the character at the specified index.

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

