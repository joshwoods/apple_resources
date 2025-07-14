

- AppKit
-  NSTextTableBlock 

Class

# NSTextTableBlock

A text block that appears as a cell in a text table.

macOS

``` source
class NSTextTableBlock
```

## Topics

### Creation

init(table: NSTextTable, startingRow: Int, rowSpan: Int, startingColumn: Int, columnSpan: Int)

Returns an initialized text table block.

### Getting the block’s enclosing table

var table: NSTextTable

Returns the table containing this text table block.

### Getting information about the block’s position in its enclosing table

var startingRow: Int

Returns the table row at which this text table block starts.

var rowSpan: Int

Returns the number of table rows spanned by this text table block.

var startingColumn: Int

Returns the table column at which this text table block starts.

var columnSpan: Int

Returns the number of table columns spanned by this text table block.

## Relationships

### Inherits From

- NSTextBlock

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

class NSTextList

A section of text that forms a single list.

class NSTextTable

An object that represents a text table as a whole.

class NSTextBlock

A block of text laid out in a subregion of the text container.

