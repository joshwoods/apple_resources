

- TabularData
- CSVReadingError
-  CSVReadingError.badEncoding(row:column:cellContents:) 

Case

# CSVReadingError.badEncoding(row:column:cellContents:)

An error that indicates CSV data contains an invalid UTF-8 byte sequence.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case badEncoding(
    row: Int,
    column: Int,
    cellContents: Data
)
```

## Parameters 

`row`  

The index of the row that contains the invalid sequence.

`column`  

The index of the column that contains the invalid sequence.

`cellContents`  

The data that contains the invalid sequence.

## See Also

### Getting Error Information

var column: Int?

The index of the column that contains the error.

var row: Int

The index of the row that contains the error.

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

