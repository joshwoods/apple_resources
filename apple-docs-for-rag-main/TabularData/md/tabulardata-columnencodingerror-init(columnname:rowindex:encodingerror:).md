

- TabularData
- ColumnEncodingError
-  init(columnName:rowIndex:encodingError:) 

Initializer

# init(columnName:rowIndex:encodingError:)

Creates a column encoding error.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    columnName: String,
    rowIndex: Int,
    encodingError: EncodingError
)
```

## Parameters 

`columnName`  

The name of the column with the error.

`rowIndex`  

The index of the column’s element with the error.

`encodingError`  

An underlying encoding error.

