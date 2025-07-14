

- AppKit
- NSParagraphStyle
-  NSParagraphStyle.TextTabType 

Enumeration

# NSParagraphStyle.TextTabType

Constants that specify the type of tab stop.

macOS

``` source
enum TextTabType
```

## Overview

The following mappings define the conversions between text alignment in NSTextTab and tab stop types that NSTextTab defines:

| Alignment | Tab stop type |
|----|----|
| NSTextAlignment.left | NSParagraphStyle.TextTabType.leftTabStopType |
| NSTextAlignment.right | NSParagraphStyle.TextTabType.rightTabStopType |
| NSTextAlignment.center | NSParagraphStyle.TextTabType.centerTabStopType |
| NSTextAlignment.justified | NSParagraphStyle.TextTabType.leftTabStopType |
| NSTextAlignment.natural | NSParagraphStyle.TextTabType.leftTabStopType, or NSParagraphStyle.TextTabType.rightTabStopType, depending on the user setting. |
| NSTextAlignment.right with a terminator | NSParagraphStyle.TextTabType.decimalTabStopType |

## Topics

### Constants

case leftTabStopType

A left-aligned tab stop.

case rightTabStopType

A right-aligned tab stop.

case centerTabStopType

A center-aligned tab stop.

case decimalTabStopType

A tab stop that aligns columns of numbers to each number’s decimal point.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing tab information

var tabStops: [NSTextTab]

The text tab objects that represent the paragraph’s tab stops.

var defaultTabInterval: CGFloat

The documentwide default tab interval.

