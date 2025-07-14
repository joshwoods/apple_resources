

- TabularData
- CSVWritingError
-  column 

Instance Property

# column

The index of the column that contains the error.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var column: String? { get }
```

## See Also

### Getting Error Information

var row: Int

The index of the row that contains the error.

case badEncoding(row: Int, column: String, Data)

An error that indicates CSV data contains an invalid UTF-8 byte sequence.

