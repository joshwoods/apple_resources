

- TabularData
- CSVWritingError
-  row 

Instance Property

# row

The index of the row that contains the error.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var row: Int { get }
```

## See Also

### Getting Error Information

var column: String?

The index of the column that contains the error.

case badEncoding(row: Int, column: String, Data)

An error that indicates CSV data contains an invalid UTF-8 byte sequence.

