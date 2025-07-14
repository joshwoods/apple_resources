

- Foundation
- NSAttributedString
-  enumerateAttribute(\_:in:options:using:) 

Instance Method

# enumerateAttribute(\_:in:options:using:)

Executes the specified closure or block for each range of a particular attribute in the attributed string.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func enumerateAttribute(
    _ attrName: NSAttributedString.Key,
    in enumerationRange: NSRange,
    options opts: NSAttributedString.EnumerationOptions = [],
    using block: (Any?, NSRange, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`attrName`  

The name of the attribute to enumerate.

`enumerationRange`  

The range over which the attribute values are enumerated.

`opts`  

The options used by the enumeration. For possible values, see NSAttributedString.EnumerationOptions.

`block`  

A closure or block to apply to ranges of the specified attribute in the attributed string, taking three arguments:

- The value for the specified attribute.

- The range of the attribute value in the attributed string.

- A reference to a Boolean value, which you can set to true within the closure to stop further processing of the attributed string.

## Discussion

If this method is called by an instance of NSMutableAttributedString, mutation (deletion, addition, or change) is allowed only if the mutation is within the range provided to the block. After a mutation, the enumeration continues with the range immediately following the processed range, adjusting for any change in length caused by the mutation. For example, if `block` is called with a range starting at location `N`, and the block deletes all the characters in the provided range, the next call will also pass `N` as the location of the range.

## See Also

### Getting attributes for a range of text

func attributes(at: Int, effectiveRange: NSRangePointer?) -> [NSAttributedString.Key : Any]

Returns the attributes for the character at the specified index.

func attributes(at: Int, longestEffectiveRange: NSRangePointer?, in: NSRange) -> [NSAttributedString.Key : Any]

Returns the attributes for the character at the specified index and, by reference, the range where the attributes apply.

func attribute(NSAttributedString.Key, at: Int, effectiveRange: NSRangePointer?) -> Any?

Returns the value for an attribute with the specified name of the character at the specified index and, by reference, the range where the attribute applies.

func attribute(NSAttributedString.Key, at: Int, longestEffectiveRange: NSRangePointer?, in: NSRange) -> Any?

Returns the value for the attribute with the specified name of the character at the specified index and, by reference, the range where the attribute applies.

func enumerateAttributes(in: NSRange, options: NSAttributedString.EnumerationOptions, using: ([NSAttributedString.Key : Any], NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes the specified closure or block for each range of attributes in the attributed string.

struct EnumerationOptions

Options for enumerating attributes.

