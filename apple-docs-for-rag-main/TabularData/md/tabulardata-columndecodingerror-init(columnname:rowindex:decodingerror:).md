

- TabularData
- ColumnDecodingError
-  init(columnName:rowIndex:decodingError:) 

Initializer

# init(columnName:rowIndex:decodingError:)

Creates a column decoding error.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    columnName: String,
    rowIndex: Int,
    decodingError: DecodingError
)
```

## Parameters 

`columnName`  

The name of the column with the error.

`rowIndex`  

The index of the column’s element with the error.

`decodingError`  

An underlying decoding error.

