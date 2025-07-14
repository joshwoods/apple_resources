

- TabularData
- ColumnDecodingError
-  columnName 

Instance Property

# columnName

The name of the column with the error.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var columnName: String
```

## See Also

### Getting Error Information

var debugDescription: String

A text representation of the column decoding error suitable for debugging.

var decodingError: DecodingError

The underlying decoding error.

var rowIndex: Int

The index of the column’s element with the error.

