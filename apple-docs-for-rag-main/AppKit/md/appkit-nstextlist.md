

- AppKit
-  NSTextList 

Class

# NSTextList

A section of text that forms a single list.

macOS 10.0+

``` source
class NSTextList
```

## Overview

The visible elements of the list, including list markers, appear in the text as they do for lists created by hand. The list object, however, allows the list to be recognized as such by the text system. This enables automatic creation of markers and spacing. Text lists are used in HTML import and export.

Text lists appear as attributes on paragraphs, as part of the paragraph style. An NSParagraphStyle may have an array of text lists, representing the nested lists containing the paragraph, in order from outermost to innermost. For example, if list1 contains four paragraphs, the middle two of which are also in the inner list2, then the text lists array for the first and fourth paragraphs is (list1), while the text lists array for the second and third paragraphs is (list1, list2).

The methods implementing this are textLists on NSParagraphStyle, and textLists on NSMutableParagraphStyle.

In addition, NSAttributedString has convenience methods for lists, such as range(of:at:), which determines the range covered by a list, and itemNumber(in:at:), which determines the ordinal position within a list of a particular item.

## Topics

### Creating a text list

init?(coder: NSCoder)

Initializes and returns a newly allocated text list item.

convenience init(markerFormat: NSTextList.MarkerFormat, options: Int)

Returns an initialized text list.

init(markerFormat: NSTextList.MarkerFormat, options: NSTextList.Options, startingItemNumber: Int)

Returns a new text list with the format, options, and starting item number you provide.

### Working with markers

var markerFormat: NSTextList.MarkerFormat

Returns the marker format string used by the receiver.

struct MarkerFormat

Constants that describe marker symbols you can apply to list elements in text lists.

func marker(forItemNumber: Int) -> String

Returns the computed value for a specific ordinal position in the list.

### Getting list options

var isOrdered: Bool

var listOptions: NSTextList.Options

Returns the list options mask value of the receiver.

struct Options

Values that available options for text list items.

### Managing item numbering

var startingItemNumber: Int

Sets the starting item number for the text list.

### Constants

The following constant specifies an option mask used with init(markerFormat:options:).

static var prependEnclosingMarker: NSTextList.Options

Specifies that a nested list should include the marker for its enclosing superlist before its own marker.

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

class NSTextTab

A tab in a paragraph.

class NSTextTable

An object that represents a text table as a whole.

class NSTextTableBlock

A text block that appears as a cell in a text table.

class NSTextBlock

A block of text laid out in a subregion of the text container.

