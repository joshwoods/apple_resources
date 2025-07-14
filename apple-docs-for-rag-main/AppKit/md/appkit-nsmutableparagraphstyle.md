

- AppKit
-  NSMutableParagraphStyle 

Class

# NSMutableParagraphStyle

An object for changing the values of the subattributes in a paragraph style attribute.

macOS 10.0+

``` source
class NSMutableParagraphStyle
```

## Overview

The NSMutableParagraphStyle class adds methods to its superclass, NSParagraphStyle, for changing the values of the subattributes in a paragraph style attribute. For more information, see NSParagraphStyle and NSAttributedString.

Important

Don’t mutate a paragraph style object after adding it to an attributed string. Doing so can cause your app to crash.

## Topics

### Setting style information

func setParagraphStyle(NSParagraphStyle)

Replaces the subattributes of the paragraph with those in the specified paragraph style object.

var alignment: NSTextAlignment

The text alignment of the paragraph.

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

The space after the end of the paragraph.

var paragraphSpacingBefore: CGFloat

The distance between the paragraph’s top and the beginning of its text content.

var baseWritingDirection: NSWritingDirection

The base writing direction for the paragraph.

### Specifying tab information

func addTabStop(NSTextTab)

Adds the specified tab stop to the paragraph.

func removeTabStop(NSTextTab)

Removes the first text tab with a location and type equal to the specified tab stop.

var tabStops: [NSTextTab]!

The text tab objects that represent the paragraph’s tab stops.

var defaultTabInterval: CGFloat

A number used as the document’s default tab spacing.

### Setting text blocks and lists

var textBlocks: [NSTextBlock]

The text blocks that contain the paragraph.

var textLists: [NSTextList]

The text lists that contain the paragraph.

### Setting line-break information

var lineBreakMode: NSLineBreakMode

The mode for breaking lines in the paragraph.

var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy

The strategies that the text system may use to break lines while laying out the paragraph.

var hyphenationFactor: Float

The paragraph’s threshold for hyphenation.

var usesDefaultHyphenation: Bool

var tighteningFactorForTruncation: Float

The threshold for using tightening as an alternative to truncation.

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that indicates whether the system tightens intercharacter spacing before truncating text.

### Setting HTML header level

var headerLevel: Int

The paragraph’s header level for HTML generation.

## Relationships

### Inherits From

- NSParagraphStyle

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

class NSParagraphStyle

The paragraph or ruler attributes for an attributed string.

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

