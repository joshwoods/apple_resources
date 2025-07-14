

- Foundation
- NSAttributedString
-  NSAttributedString.EnumerationOptions 

Structure

# NSAttributedString.EnumerationOptions

Options for enumerating attributes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct EnumerationOptions
```

## Overview

These constants describe the options available to the enumerateAttribute(_:in:options:using:) and enumerateAttributes(in:options:using:) methods.

## Topics

### Getting the enumeration options

static var reverse: NSAttributedString.EnumerationOptions

Causes the enumeration to occur in reverse.

static var longestEffectiveRangeNotRequired: NSAttributedString.EnumerationOptions

If `NSAttributedStringEnumerationLongestEffectiveRangeNotRequired` option is supplied, then the longest effective range computation is not performed; the blocks may be invoked with consecutive attribute runs that have the same value.

### Creating an enumeration option

init(rawValue: UInt)

static var reverse: NSAttributedString.EnumerationOptions

Causes the enumeration to occur in reverse.

static var longestEffectiveRangeNotRequired: NSAttributedString.EnumerationOptions

If `NSAttributedStringEnumerationLongestEffectiveRangeNotRequired` option is supplied, then the longest effective range computation is not performed; the blocks may be invoked with consecutive attribute runs that have the same value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

func enumerateAttribute(NSAttributedString.Key, in: NSRange, options: NSAttributedString.EnumerationOptions, using: (Any?, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes the specified closure or block for each range of a particular attribute in the attributed string.

func enumerateAttributes(in: NSRange, options: NSAttributedString.EnumerationOptions, using: ([NSAttributedString.Key : Any], NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes the specified closure or block for each range of attributes in the attributed string.

