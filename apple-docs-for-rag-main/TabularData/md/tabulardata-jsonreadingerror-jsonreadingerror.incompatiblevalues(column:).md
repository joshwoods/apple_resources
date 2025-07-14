

- TabularData
- JSONReadingError
-  JSONReadingError.incompatibleValues(column:) 

Case

# JSONReadingError.incompatibleValues(column:)

An error that occurs when the JSON data contains incompatible values in a column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case incompatibleValues(column: String)
```

## Parameters 

`column`  

The name of the column that contains the incompatible values.

## See Also

### Getting Error Information

case failedToParse(row: Int, column: String, type: JSONType, contents: String)

An error that occurs when a JSON value fails to parse as the specified type.

case unsupportedStructure

An error that occurs when the JSON structure is incompatible with a data frame.

case wrongType(row: Int, column: String, expectedType: JSONType, value: any Sendable)

An error that occurs when the JSON data contains a value of the wrong type for a type-constrained column.

