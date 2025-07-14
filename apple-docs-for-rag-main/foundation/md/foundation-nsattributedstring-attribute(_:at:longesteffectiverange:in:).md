

- Foundation
- NSAttributedString
-  attribute(\_:at:longestEffectiveRange:in:) 

Instance Method

# attribute(\_:at:longestEffectiveRange:in:)

Returns the value for the attribute with the specified name of the character at the specified index and, by reference, the range where the attribute applies.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func attribute(
    _ attrName: NSAttributedString.Key,
    at location: Int,
    longestEffectiveRange range: NSRangePointer?,
    in rangeLimit: NSRange
) -> Any?
```

## Parameters 

`attrName`  

The name of an attribute.

`location`  

The index at which to test for `attributeName`.

`range`  

If non-`NULL`:

- If the named attribute exists at `index`, upon return `aRange` contains the full range over which the value of the named attribute is the same as that at `index`, clipped to `rangeLimit`.

- If the named attribute does not exist at `index`, upon return `aRange` contains the full range over which the attribute does not exist, clipped to `rangeLimit`.

If you don’t need this value, pass `NULL`.

`rangeLimit`  

The range over which to search for continuous presence of `attributeName`. This value must not exceed the bounds of the receiver.

## Return Value

The value for the attribute named `attributeName` of the character at `index`, or `nil` if there is no such attribute.

## Discussion

Raises an rangeException if `index` or any part of `rangeLimit` lies beyond the end of the receiver’s characters.

If you don’t need the longest effective range, it’s far more efficient to use the attribute(_:at:effectiveRange:) method to retrieve the attribute value.

For a list of possible attributes, see NSAttributedString.Key.

## See Also

### Getting attributes for a range of text

func attributes(at: Int, effectiveRange: NSRangePointer?) -> [NSAttributedString.Key : Any]

Returns the attributes for the character at the specified index.

func attributes(at: Int, longestEffectiveRange: NSRangePointer?, in: NSRange) -> [NSAttributedString.Key : Any]

Returns the attributes for the character at the specified index and, by reference, the range where the attributes apply.

func attribute(NSAttributedString.Key, at: Int, effectiveRange: NSRangePointer?) -> Any?

Returns the value for an attribute with the specified name of the character at the specified index and, by reference, the range where the attribute applies.

func enumerateAttribute(NSAttributedString.Key, in: NSRange, options: NSAttributedString.EnumerationOptions, using: (Any?, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes the specified closure or block for each range of a particular attribute in the attributed string.

func enumerateAttributes(in: NSRange, options: NSAttributedString.EnumerationOptions, using: ([NSAttributedString.Key : Any], NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes the specified closure or block for each range of attributes in the attributed string.

struct EnumerationOptions

Options for enumerating attributes.

