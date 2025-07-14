

- TabularData
-  FormattingOptions 

Structure

# FormattingOptions

A set of parameters that indicate how to present the contents of data frame or column types to a printable string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct FormattingOptions
```

## Topics

### Creating the Options Object

init()

Creates a formatting options instance with default parameters.

init(locale: Locale)

Creates a formatting options instance with a locale.

init(maximumLineWidth: Int, maximumCellWidth: Int, maximumRowCount: Int, includesColumnTypes: Bool)

Creates a formatting options instance.

### Getting the Properties

var dateFormatStyle: Date.FormatStyle

The date format style.

var floatingPointFormatStyle: FloatingPointFormatStyle&lt;Double>

The floating point format style.

var includesColumnTypes: Bool

A Boolean value that indicates whether the description includes the column types.

var integerFormatStyle: IntegerFormatStyle&lt;Int>

The integer format style.

var locale: Locale

The locale.

var maximumCellWidth: Int

The largest number of characters a description can generate per cell.

var maximumLineWidth: Int

The largest number of characters a description can generate per line.

var maximumRowCount: Int

The largest number of rows a description can generate.

### Instance Properties

var includesRowAndColumnCounts: Bool

A Boolean value that indicates whether the description includes the number of rows and columns.

var includesRowIndices: Bool

A Boolean value that indicates whether the description includes the row indices.

## See Also

### Supporting Types

enum Order

A type that represents a sort ordering.

struct ColumnID

A column identifier that stores a column’s name and the type of its elements.

