

- TabularData
-  CSVReadingError 

Enumeration

# CSVReadingError

A CSV reading error.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum CSVReadingError
```

## Topics

### Getting Error Information

var column: Int?

The index of the column that contains the error.

var row: Int

The index of the row that contains the error.

case badEncoding(row: Int, column: Int, cellContents: Data)

An error that indicates CSV data contains an invalid UTF-8 byte sequence.

case failedToParse(row: Int, column: Int, type: CSVType, cellContents: Data)

An error that indicates the CSV reader can’t parse data in the file.

case misplacedQuote(row: Int, column: Int)

An error that indicates the CSV data contains a misplaced quote.

case missingColumn(columnName: String)

An error that indicates the CSV is missing a required column.

case unsupportedEncoding(String)

An error that indicates the CSV reader doesn’t support an encoding.

case wrongNumberOfColumns(row: Int, columns: Int, expected: Int)

An error that indicates the CSV data contains a row with a mismatched number of columns.

### Enumeration Cases

case outOfBounds(requested: Int, actual: Int)

An error that indicates that the read operation requested rows beyond the end of the CSV file.

case unsupportedColumnType(columnIndex: Int, columnName: String, type: String)

An error that indicates that a column type is not one of the types supported by CSV.

### Default Implementations

CustomStringConvertible Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Error
- LocalizedError
- Sendable

## See Also

### Errors

enum JSONReadingError

A JSON reading error.

enum CSVWritingError

A CSV writing error.

struct ColumnDecodingError

A column decoding error.

struct ColumnEncodingError

A column encoding error.

enum SFrameReadingError

An error when reading a Turi Create scalable data frame.

