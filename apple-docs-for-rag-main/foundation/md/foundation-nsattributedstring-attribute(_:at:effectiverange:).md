

- Foundation
- NSAttributedString
-  attribute(\_:at:effectiveRange:) 

Instance Method

# attribute(\_:at:effectiveRange:)

Returns the value for an attribute with the specified name of the character at the specified index and, by reference, the range where the attribute applies.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func attribute(
    _ attrName: NSAttributedString.Key,
    at location: Int,
    effectiveRange range: NSRangePointer?
) -> Any?
```

## Parameters 

`attrName`  

The name of an attribute.

`location`  

The index for which to return attributes. This value must not exceed the bounds of the receiver.

Important

Raises an rangeException if `index` lies beyond the end of the receiver’s characters.

`range`  

If non-`NULL`:

- If the named attribute exists at `index`, upon return `aRange` contains a range over which the named attribute’s value applies.

- If the named attribute does not exist at `index`, upon return `aRange` contains the range over which the attribute does not exist.

The range isn’t necessarily the maximum range covered by `attributeName`, and its extent is implementation-dependent. If you need the maximum range, use attribute(_:at:longestEffectiveRange:in:). If you don’t need this value, pass `NULL`.

## Return Value

The value for the attribute named `attrName` of the character at `location`, or `nil` if there is no such attribute.

## Discussion

For a list of possible attributes, see NSAttributedString.Key.

## See Also

### Getting attributes for a range of text

func attributes(at: Int, effectiveRange: NSRangePointer?) -> [NSAttributedString.Key : Any]

Returns the attributes for the character at the specified index.

func attributes(at: Int, longestEffectiveRange: NSRangePointer?, in: NSRange) -> [NSAttributedString.Key : Any]

Returns the attributes for the character at the specified index and, by reference, the range where the attributes apply.

func attribute(NSAttributedString.Key, at: Int, longestEffectiveRange: NSRangePointer?, in: NSRange) -> Any?

Returns the value for the attribute with the specified name of the character at the specified index and, by reference, the range where the attribute applies.

func enumerateAttribute(NSAttributedString.Key, in: NSRange, options: NSAttributedString.EnumerationOptions, using: (Any?, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes the specified closure or block for each range of a particular attribute in the attributed string.

func enumerateAttributes(in: NSRange, options: NSAttributedString.EnumerationOptions, using: ([NSAttributedString.Key : Any], NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes the specified closure or block for each range of attributes in the attributed string.

struct EnumerationOptions

Options for enumerating attributes.

