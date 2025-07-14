

- TabularData
- ColumnEncodingError
-  debugDescription 

Instance Property

# debugDescription

A text representation of the column encoding error suitable for debugging.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var debugDescription: String { get }
```

## See Also

### Getting Error Information

var columnName: String

The name of the column with the error.

var encodingError: EncodingError

The underlying encoding error.

var rowIndex: Int

The index of the column’s element with the error.

