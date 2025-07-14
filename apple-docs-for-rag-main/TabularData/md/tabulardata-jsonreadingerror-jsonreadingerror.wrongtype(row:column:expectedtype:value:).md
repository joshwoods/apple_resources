

- TabularData
- JSONReadingError
-  JSONReadingError.wrongType(row:column:expectedType:value:) 

Case

# JSONReadingError.wrongType(row:column:expectedType:value:)

An error that occurs when the JSON data contains a value of the wrong type for a type-constrained column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case wrongType(
    row: Int,
    column: String,
    expectedType: JSONType,
    value: any Sendable
)
```

## Parameters 

`row`  

The index of the row that contains the incorrect value.

`column`  

The name of the column that contains the incorrect value.

`expectedType`  

The expected type.

`value`  

The JSON value.

## See Also

### Getting Error Information

case failedToParse(row: Int, column: String, type: JSONType, contents: String)

An error that occurs when a JSON value fails to parse as the specified type.

case incompatibleValues(column: String)

An error that occurs when the JSON data contains incompatible values in a column.

case unsupportedStructure

An error that occurs when the JSON structure is incompatible with a data frame.

