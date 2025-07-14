

- Core Text
-  CTParagraphStyleSpecifier 

Enumeration

# CTParagraphStyleSpecifier

Constants used to query and modify a paragraph style object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CTParagraphStyleSpecifier
```

## Overview

Each specifier has a type and a default value associated with it. The type must always be observed when setting or fetching the value from the `CTParagraphStyle` object. In addition, some specifiers affect the behavior of both the framesetter and the typesetter, and others affect the behavior of only the framesetter, as noted in the constant descriptions.

## Topics

### Constants

case alignment

The text alignment.

case firstLineHeadIndent

The distance, in points, from the leading margin of a frame to the beginning of the paragraph’s first line.

case headIndent

The distance, in points, from the leading margin of a text container to the beginning of lines other than the first.

case tailIndent

The distance, in points, from the margin of a frame to the end of lines.

case tabStops

The text tab objects, sorted by location, that define the tab stops for the paragraph style.

case defaultTabInterval

The document-wide default tab interval.

case lineBreakMode

The mode that should be used to break lines when laying out the paragraph’s text.

case lineHeightMultiple

The line height multiple.

case maximumLineHeight

The maximum height that any line in the frame will occupy, regardless of the font size or size of any attached graphic.

case minimumLineHeight

The minimum height that any line in the frame will occupy, regardless of the font size or size of any attached graphic.

case lineSpacing

The space in points added between lines within the paragraph (commonly known as leading).

Deprecated

case paragraphSpacing

The space added at the end of the paragraph to separate it from the following paragraph.

case paragraphSpacingBefore

The distance between the paragraph’s top and the beginning of its text content.

case baseWritingDirection

The base writing direction of the lines.

case maximumLineSpacing

The maximum space in points between lines within the paragraph (commonly known as leading).

case minimumLineSpacing

The minimum space in points between lines within the paragraph (commonly known as leading).

case lineSpacingAdjustment

The space in points added between lines within the paragraph (commonly known as leading).

case count

The number of style specifiers.

### Enumeration Cases

case lineBoundsOptions

Options that control the alignment of the line edges with the leading and trailing margins.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum CTTextAlignment

Constants that specify text alignment.

enum CTLineBreakMode

These constants specify what happens when a line is too long for its frame.

enum CTWritingDirection

These constants specify the writing direction.

