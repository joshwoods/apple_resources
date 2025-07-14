

- AppKit
-  NSParagraphStyle 

Class

# NSParagraphStyle

The paragraph or ruler attributes for an attributed string.

macOS 10.0+

``` source
class NSParagraphStyle
```

## Overview

An NSParagraphStyle object stores formatting information for a paragraph of text. The formatting information includes the amount of space between lines, indentations for lines of text, line heights, tab-stop positions, and more. Apply paragraph styles to the text of an attributed string by adding the paragraphStyle attribute and setting its value to an instance of this class. The text-rendering system uses the paragraph style information in an attributed string to lay out and render the text.

The NSParagraphStyle class manages an immutable set of style information, but you can create an NSMutableParagraphStyle when you want to modify the style information before applying it to your text.

## Topics

### Creating a paragraph style

class var `default`: NSParagraphStyle

The default paragraph style.

### Accessing style information

var alignment: NSTextAlignment

The text alignment of the paragraph.

enum NSTextAlignment

Constants that specify text alignment.

var firstLineHeadIndent: CGFloat

The indentation of the first line of the paragraph.

var headIndent: CGFloat

The indentation of the paragraph’s lines other than the first.

var tailIndent: CGFloat

The trailing indentation of the paragraph.

var lineHeightMultiple: CGFloat

The line height multiple.

var maximumLineHeight: CGFloat

The paragraph’s maximum line height.

var minimumLineHeight: CGFloat

The paragraph’s minimum line height.

var lineSpacing: CGFloat

The distance in points between the bottom of one line fragment and the top of the next.

var paragraphSpacing: CGFloat

Distance between the bottom of this paragraph and top of next.

var paragraphSpacingBefore: CGFloat

The distance between the paragraph’s top and the beginning of its text content.

### Accessing tab information

var tabStops: [NSTextTab]

The text tab objects that represent the paragraph’s tab stops.

enum TextTabType

Constants that specify the type of tab stop.

var defaultTabInterval: CGFloat

The documentwide default tab interval.

### Getting text block and list information

var textBlocks: [NSTextBlock]

The text blocks that contain the paragraph.

var textLists: [NSTextList]

The text lists that contain the paragraph.

### Getting line-break information

var lineBreakMode: NSLineBreakMode

The mode for breaking lines in the paragraph that don’t fit within a container.

enum NSLineBreakMode

Constants that specify what happens when a line is too long for a container.

var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy

The strategy for breaking lines while laying out paragraphs.

struct LineBreakStrategy

Constants that specify how the text system breaks lines while laying out paragraphs.

var hyphenationFactor: Float

The paragraph’s threshold for hyphenation.

var usesDefaultHyphenation: Bool

A Boolean value that indicates whether the paragraph style uses the system hyphenation settings.

var tighteningFactorForTruncation: Float

The threshold for using tightening as an alternative to truncation.

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that indicates whether the system tightens character spacing before truncating text.

### Getting the html header level

var headerLevel: Int

The paragraph’s header level for HTML generation.

### Determining writing direction

class func defaultWritingDirection(forLanguage: String?) -> NSWritingDirection

Returns the default writing direction for the specified language.

var baseWritingDirection: NSWritingDirection

The base writing direction for the paragraph.

enum NSWritingDirection

Constants that specify the writing direction.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSMutableParagraphStyle

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

### Formatting and attributes

class NSMutableParagraphStyle

An object for changing the values of the subattributes in a paragraph style attribute.

class NSTextTab

A tab in a paragraph.

class NSTextList

A section of text that forms a single list.

class NSTextTable

An object that represents a text table as a whole.

class NSTextTableBlock

A text block that appears as a cell in a text table.

class NSTextBlock

A block of text laid out in a subregion of the text container.

