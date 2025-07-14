

- UIKit
-  NSTextTab 

Class

# NSTextTab

A tab in a paragraph.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSTextTab
```

## Overview

A text tab represents a tab in an NSParagraphStyle object, storing an alignment type and location. NSTextTab objects are most frequently used with the TextKit system and with NSRulerView and NSRulerMarker objects.

The text system supports four alignment types: left, center, right, and decimal (based on the decimal separator character of the locale in effect). These alignment types are absolute, not based on the line sweep direction of text. For example, tabbed text is always positioned to the left of a right-aligned tab, whether the line sweep direction is left to right or right to left. A tab’s location, on the other hand, is relative to the back margin. A tab set at 1.5”, for example, is at 1.5” from the right in right to left text.

## Topics

### Creating a text tab

init(textAlignment: NSTextAlignment, location: CGFloat, options: [NSTextTab.OptionKey : Any])

Initializes a text tab with the specified text alignment, location, and options.

### Getting tab stop information

var location: CGFloat

The text tab’s ruler location relative to the back margin.

### Getting text tab information

var alignment: NSTextAlignment

The text alignment of the text tab.

var options: [NSTextTab.OptionKey : Any]

The dictionary of attributes for the text tab.

class func columnTerminators(for: Locale?) -> CharacterSet

Returns the column terminators for the specified locale.

### Constants

enum TextTabType

Constants that specify the type of tab stop.

struct OptionKey

The terminating character for a tab column.

### Deprecated

convenience init(type: NSParagraphStyle.TextTabType, location loc: CGFloat)

Initializes a newly allocated text tab with the specified alignment and location.

var tabStopType: NSParagraphStyle.TextTabType { get }

The text tab’s type of tab stop.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Formatting and attributes

class NSParagraphStyle

The paragraph or ruler attributes for an attributed string.

class NSMutableParagraphStyle

An object for changing the values of the subattributes in a paragraph style attribute.

class NSTextList

A section of text that forms a single list.

