

- Foundation
-  NSMutableAttributedString 

Class

# NSMutableAttributedString

A mutable string with associated attributes (such as visual style, hyperlinks, or accessibility data) for portions of its text.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSMutableAttributedString
```

## Overview

The `NSMutableAttributedString` class declares additional methods for mutating the content of an attributed string. You can add and remove characters (raw strings) and attributes separately or together as attributed strings. See the class description for NSAttributedString for more information about attributed strings.

`NSMutableAttributedString` adds two primitive methods to those of `NSAttributedString`. These primitive methods provide the basis for all the other methods in its class. The primitive replaceCharacters(in:with:) method replaces a range of characters with those from a string, leaving all attribute information outside that range intact. The primitive setAttributes(_:range:) method sets attributes and values for a given range of characters, replacing any previous attributes and values for that range.

In macOS, AppKit also uses NSParagraphStyle and its subclass NSMutableParagraphStyle to encapsulate the paragraph or ruler attributes used by the `NSAttributedString` classes.

Note that the default font for `NSAttributedString` objects is Helvetica 12-point, which may differ from the macOS system font, so you may wish to create the string with non-default attributes suitable for your application using, for example, init(string:attributes:).

iOS Note

In iOS, this class is used primarily in conjunction with the Core Text framework.

`NSMutableAttributedString` is “toll-free bridged” with its Core Foundation counterpart, CFMutableAttributedString. See Toll-Free Bridging for more information.

## Topics

### Retrieving Character Information

var mutableString: NSMutableString

The character contents of the receiver as a mutable string object.

### Changing Characters

func replaceCharacters(in: NSRange, with: String)

Replaces the characters in the given range with the characters of the given string.

func deleteCharacters(in: NSRange)

Deletes the characters in the given range along with their associated attributes.

### Changing Attributes

func setAttributes([NSAttributedString.Key : Any]?, range: NSRange)

Sets the attributes for the characters in the specified range to the specified attributes.

func addAttribute(NSAttributedString.Key, value: Any, range: NSRange)

Adds an attribute with the given name and value to the characters in the specified range.

func addAttributes([NSAttributedString.Key : Any], range: NSRange)

Adds the given collection of attributes to the characters in the specified range.

func removeAttribute(NSAttributedString.Key, range: NSRange)

Removes the named attribute from the characters in the specified range.

func applyFontTraits(NSFontTraitMask, range: NSRange)

Applies the specified font-related attributes to characters in the string.

func setAlignment(NSTextAlignment, range: NSRange)

Sets the alignment characteristic of the paragraph style attribute for the specified range of text.

func setBaseWritingDirection(NSWritingDirection, range: NSRange)

Sets the base writing direction for the characters to the specified direction.

func subscriptRange(NSRange)

Decrements the value of the superscript attribute for characters in the specified range by one.

func superscriptRange(NSRange)

Increments the value of the superscript attribute for characters in the specified range by one.

func unscriptRange(NSRange)

Removes the superscript attribute from the characters in the specified range.

### Changing Characters and Attributes

func append(NSAttributedString)

Adds the characters and attributes of a given attributed string to the end of the receiver.

func insert(NSAttributedString, at: Int)

Inserts the characters and attributes of the given attributed string into the receiver at the given index.

func replaceCharacters(in: NSRange, with: NSAttributedString)

Replaces the characters and attributes in a given range with the characters and attributes of the given attributed string.

func setAttributedString(NSAttributedString)

Replaces the receiver’s entire contents with the characters and attributes of the given attributed string.

### Grouping Changes

func beginEditing()

Begins the buffering of changes to the string’s characters and attributes.

func endEditing()

Ends the buffering of changes to the string’s characters and attributes.

### Updating Attachment Contents

func updateAttachments(fromPath: String)

Updates all attachments based on files contained in the RTFD file package at the specified file path.

### Fixing Attributes After Changes

func fixAttributes(in: NSRange)

Cleans up font, paragraph style, and attachment attributes within the given range.

func fixAttachmentAttribute(in: NSRange)

Cleans up attachment attributes in the specified range and removes all attachment attributes assigned to characters except the designated attachment character.

func fixFontAttribute(in: NSRange)

Fixes the font attribute in the specified range and assigns default fonts where appropriate.

func fixParagraphStyleAttribute(in: NSRange)

Fixes the paragraph style attributes in the specified range and assigns a paragraph style to all characters in the paragraph.

### Reading Content

func read(from: Data, options: [NSAttributedString.DocumentReadingOptionKey : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) throws

Sets the contents of the attributed string using the specified data object`.`

func read(from: URL, options: [NSAttributedString.DocumentReadingOptionKey : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) throws

Sets the contents of attributed string using the contents of the specified file.

### Deprecated

func read(from: Data, options: [AnyHashable : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) -> Bool

Sets the contents of the receiver from the specified data object`.`

Deprecated

func read(from: URL, options: [AnyHashable : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) -> Bool

Sets the contents of receiver from the file at the specified URL.

Deprecated

func read(fromFileURL: URL, options: [AnyHashable : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) throws

Sets the contents of the receiver from the file at the given URL.

Deprecated

## Relationships

### Inherits From

- NSAttributedString

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Strings with Metadata

struct AttributedString

A value type for a string with associated attributes for portions of its text.

struct AttributedSubstring

A portion of an attributed string.

Attributed String Supporting Types

Types that the attributed string, attributed substring, and helper types extend or conform to, for sharing common functionality.

class NSAttributedString

A string of text that manages data, layout, and stylistic information for ranges of characters to support rendering.

